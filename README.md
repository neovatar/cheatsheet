## Docker

| Name                     | Command                                                                          | 
| ------------------------ |----------------------------------------------------------------------------------|
| condensed docker ps      | `docker ps --format "table {{.ID}}\t{{.Names}}\t{{.Status}}"`                    |

## K8s
| Name                     | Command                                                                          | 
| ------------------------ |----------------------------------------------------------------------------------|
| interactive k8s pod      | kubectl run my-pod --restart=Never -it --rm --image ubuntu -- bash               |
