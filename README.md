# Cloud

docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Cloud202402' -p 1433:1433 --name sqlserver2024 -d mcr.microsoft.com/mssql/server:2022-latest
docker commit b48335adfd9f146635e65ea2fe6d21fd90f6f15c14e9cf620293f54222f2a12f cloud2024:1.0
docker tag cloud2024:1.0 hvmiranda/cloud
docker push hvmiranda/cloud

