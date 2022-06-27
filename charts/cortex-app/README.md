##### Install cortex-app default values
1. `N=cortex-development && helm upgrade cortex-development cortex-app -i -n $N`
1. Verify `kubectl port-forward -n $N cortex-ui-deployment-856577b4d8-gm5s8 8080:80`


##### Install cortex-app pretty-solution.com values
1. `N=cortex-development && helm upgrade cortex-development cortex-app -i -n $N -f pretty-values.yaml`

export ConnectionStrings__BaseClientConnection="Data Source=3.tcp.eu.ngrok.io,23790;TrustServerCertificate=True;Initial Catalog=ClientEX;User ID=cortexdev_admin;Password=9Rp4s@zu5K;"
export ConnectionStrings__MasterConnection="Data Source=3.tcp.eu.ngrok.io,23790;TrustServerCertificate=True;Initial Catalog=Cortex;User ID=cortexdev_admin;Password=9Rp4s@zu5K;"
export ConnectionStrings__DeploymentConnection="Data Source=3.tcp.eu.ngrok.io,23790;TrustServerCertificate=True;Initial Catalog=ClientEX;User ID=cortexdev_admin;Password=9Rp4s@zu5K;"
export ConnectionStrings__AdminConnection="Data Source=3.tcp.eu.ngrok.io,23790;TrustServerCertificate=True;Initial Catalog=CortexAdminDemo;User ID=cortexdev_admin;Password=9Rp4s@zu5K;"
