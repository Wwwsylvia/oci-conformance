# ACR

## Conformance Tests

```bash
git clone https://github.com/opencontainers/distribution-spec.git
cd distribution-spec/conformance
go test -c
OCI_TEST_PULL=1 OCI_TEST_PUSH=1 OCI_TEST_CONTENT_DISCOVERY=1 OCI_TEST_CONTENT_MANAGEMENT=1 OCI_ROOT_URL="https://${acr_name}.azurecr.io" OCI_NAMESPACE="${test_repo}" OCI_USERNAME="${test_username}" OCI_PASSWORD="${test_password}" ./conforma
nce.test
```


