## vitesse-sdk

Organization managed by *vitesse-sdk-admin* to host private NuGet packages.

Contact sdk at vitesse.io for further details or to request access to NuGet packages.

### Troubleshoot NuGet Package Access

Provided a token with `packages:read` access has been issued, test access to the organization's private NuGet feed with
```
curl --silent --header "Authorization: Bearer your_token" "https://api.github.com/users/vitesse-sdk/packages?package_type=nuget"
```

If the specified `your_token` has read permissions on packages at *vitesse-sdk* organization, a list of private packages should be listed. Otherwise it will be empty.

With this basic test, it can be verified whether a specific token is active or has been revoked.
