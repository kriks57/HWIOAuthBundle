Step 2x: Setup Apple
=====================
First you will have to register your application on Apple Developers website. Check out the
documentation for more information: https://help.apple.com/developer-account/?lang=en#/devde676e696

Next configure a resource owner of type `apple` with appropriate
`client_id`, `client_secret` and `scope`.
Example `scope` values include:
* `name`
* `email`
``` yaml
# config/packages/hwi_oauth.yaml

hwi_oauth:
    resource_owners:
        any_name:
            type:                apple
            client_id:           <client_id>
            client_secret:       <client_secret>
            scope:               "name email"
```

When you're done. Continue by configuring the security layer or go back to
setup more resource owners.

- [Step 2: Configuring resource owners (Facebook, GitHub, Google, Windows Live and others](../2-configuring_resource_owners.md)
- [Step 3: Configuring the security layer](../3-configuring_the_security_layer.md).
