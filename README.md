# Standard Demo Bundle

This is a fully working Entando Bundle for recreating the Standard Demo Experience.
Just install this using `entando-component-manager >= 6.3.0`

### Dump Command:
This bundle was 95% generated using [entando-bundle-cli](https://github.com/entando-k8s/entando-bundle-cli) and extracting most components from the following environment:
```
$ entando-bundle from-env \
    --env env.json \
    --code standard-demo-bundle \
    --description "Standard Demo Bundle"
```

*env.json*
```
{
    "coreBaseApi": "http://quickstart-entando.apps.rd.entando.org/entando-de-app",
    "k8ssvcApi": "http://quickstart-eci-entando.apps.rd.entando.org/k8s",
    "clientId": "entando-bundle-cli",
    "clientSecret": "<insert_secret_here>"
}
```

or use the interactive command to execute the cli interactive version:
```
$ entando-bundle
? What do you want to do? Create a new bundle using components from an environment
? Please select an env.json file with the environment variables: env.json
? Which type of components do you want to add to the bundle? All components
Collecting all components from the provided environment...
? Do you want to generate the Bundle with the selected components? Yes
? Where do you want to generate the Bundle? ./
? What's the code for the Bundle? standard-demo-bundle
? Please add a description to the Bundle: Standard Demo Bundle
Generating bundle...
```
