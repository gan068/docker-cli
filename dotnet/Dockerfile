FROM --platform=$BUILDPLATFORM mcr.microsoft.com/dotnet/sdk:7.0 AS build

WORKDIR /src

COPY src ./

RUN dotnet publish -c release --self-contained false -o /src/out

FROM --platform=$BUILDPLATFORM mcr.microsoft.com/dotnet/aspnet:7.0 AS base

WORKDIR /app

COPY --from=build /src/out ./

ENTRYPOINT ["dotnet", "demo.dll"]

