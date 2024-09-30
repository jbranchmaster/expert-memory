# Delete Objects of CRDs

- This command deletes Objects the CRDs. 
- Get all the CRDs based on a group-id and delete them.
- [Source](https://stackable.tech/en/deleting-custom-resources-in-a-kubernetes-namespace/)
```
kubectl api-resources | grep group.id
..result

kubectl delete <crd-name> --all
```
