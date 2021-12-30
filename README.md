# az-private-linky-integration-suite
SAP Integration Suite artifacts to get you started with SAP BTP Private Link Service for Azure.

Find my blog post series on the topic [here](https://blogs.sap.com/2021/07/13/btp-private-linky-swear-with-azure-business-as-usual-for-iflows/).

The package contains two iFlows. One configured against the CAP implementation and one for Java. They differ due to the chosen router configuration. They can be adapted as required.

Additional Resources |
--- |
[CAP backend Project](https://github.com/MartinPankraz/az-private-linky-cap) |
[Java backend Project using SAP Cloud SDK](https://github.com/MartinPankraz/az-private-linky) |
[Fiori Project consuming above backends](https://github.com/MartinPankraz/az-products-ui) |
[SAP's official blog](https://blogs.sap.com/2021/06/28/sap-private-link-service-beta-is-available/) |

We used the `/sap/opu/odata/sap/epm_ref_apps_prod_man_srv` OData service for this project.

## Project context
[Azure Private Link Service](https://docs.microsoft.com/en-us/azure/private-link/private-link-service-overview) allows private connectivity between resources running on Azure in different environments. That includes SAP's Business Technology Platform when provisioned on Azure. SAP made that functionality available via a CloudFoundry Service.

Meaning you get now a managed component to expose your SAP backends to BTP on Azure without the need for a Cloud Connector. For this example, we developed against S4 primarily but anything executable in a service behind the Azure load balancer would be reachable. That involves for instance ECC, BO, PI/PO, SolMan, SAP CAR etc.

![Architecture overview](/linky-cpi-overview.png)

Reach out via the [GitHub Issues page](https://github.com/MartinPankraz/az-private-linky-integration-suite/issues) of this reposto talk about it some more :-)
