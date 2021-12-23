FROM mcr.microsoft.com/dotnet/runtime:3.1
WORKDIR /app
COPY /bin/Release/netcoreapp3.1/publish /app/
ENTRYPOINT ["dotnet", "DockerNetCoreConsole.dll"]

# docker build -t dockernetcoreconsole .
# docker build -t dockernetcoreconsole:v1 .
# docker images

# cls

# docker create --name dockernetcoreconsole-container dockernetcoreconsole
# docker ps -a
# docker start dockernetcoreconsole-container
# docker ps
# docker stop dockernetcoreconsole-container

# cls

# docker attach 615
# docker attach dockernetcoreconsole-container

# cls

# docker run --name dockernetcoreconsole-container3 615
# docker run --name dockernetcoreconsole-container3 dockernetcoreconsole
# docker rm 615
# docker rm dockernetcoreconsole-container3
# docker run --rm --name dockernetcoreconsole-container-1 dockernetcoreconsole

# cls

# docker ps -a
# docker images
# docker rmi 9b5
# docker rmi dockernetcoreconsole

# cls

# docker build -t docker-console-app:v1 .
# docker run --name docker-console-container-1 docker-console-app:v1
# docker stop dockernetcoreconsole-container
# docker rm docker-console-container-1
# docker rm docker-console-container-1 --force
# docker rmi docker-console-app:v1
# docker stop dockernetcoreconsole-container
# docker rmi docker-console-app:v1 --force

# docker pull mcr.microsoft.com/dotnet/sdk:3.1
# docker pull mcr.microsoft.com/dotnet/sdk:6.0

# docker pull busybox
# docker images
# docker tag busybox iskylarkus/docker-console:v1
# docker login
# docker push iskylarkus/docker-console:v1
# docker tag busybox iskylarkus/docker-console:v2
# docker images
# docker push iskylarkus/docker-console:v1




#See https://aka.ms/containerfastmode to understand how Visual Studio uses this Dockerfile to build your images for faster debugging.

#FROM mcr.microsoft.com/dotnet/runtime:3.1 AS base
#WORKDIR /app

#FROM mcr.microsoft.com/dotnet/sdk:3.1 AS build
#WORKDIR /src
#COPY ["DockerNetCoreConsole/DockerNetCoreConsole.csproj", "DockerNetCoreConsole/"]
#RUN dotnet restore "DockerNetCoreConsole/DockerNetCoreConsole.csproj"
#COPY . .
#WORKDIR "/src/DockerNetCoreConsole"
#RUN dotnet build "DockerNetCoreConsole.csproj" -c Release -o /app/build

#FROM build AS publish
#RUN dotnet publish "DockerNetCoreConsole.csproj" -c Release -o /app/publish

#FROM base AS final
#WORKDIR /app
#COPY --from=publish /app/publish .
#ENTRYPOINT ["dotnet", "DockerNetCoreConsole.dll"]