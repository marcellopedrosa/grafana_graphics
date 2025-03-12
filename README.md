#1. JVM MEMORY Graphic#

G1 Eden Space MB

(jvm_memory_used_bytes{application="rest-app",id="G1 Eden Space",job="rest-app"})/1048576

G1 Survivor Space MB

jvm_memory_used_bytes{application="rest-app",id="G1 Survivor Space",job="rest-app"}/1048576

#2. STATUS HTTP ERRORS Graphic#

http_server_requests_seconds_max{application="rest-app", exception!="BadCredentialsException", status="500", job="rest-app"}
http_server_requests_seconds_max{application="rest-app", status="403", method!="OPTIONS", uri!="/actuator/prometheus", job="rest-app"}
http_server_requests_seconds_max{application="rest-app", status="404",  job="rest-app"}

#3. UP TIME Graphic#

process_uptime_seconds{application="rest-app",job="rest-app"}
