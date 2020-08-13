Create the resources.
```bash
kubectl apply -f .
```

Both bods will run the endless loop writing events into the log file. Run the following to make sure that everything works:
```bash
kubectl exec -it app1 -- tail /data/out1.txt
kubectl exec -it app2 -- tail /data/out1.txt
```
