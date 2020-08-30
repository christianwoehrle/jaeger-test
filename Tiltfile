print('Hello Tiltfile')


docker_build( 'christianwoehrle/jaeger-test', '.')

k8s_yaml('jaeger-client.yaml')
k8s_yaml('jaeger-service.yaml')
k8s_yaml('jaeger-client2.yaml')
k8s_yaml('jaeger-service2.yaml')


k8s_resource(workload='jaeger-client', port_forwards='9000:9000')
k8s_resource(workload='jaeger-client2', port_forwards='9001:9000')
#k8s_resource(new_name='duh', objects=['svc/jaeger-client'], port_forwards=[9000]) 
#k8s_resource('name', 'yaml', port_forwards=[8080]) 
