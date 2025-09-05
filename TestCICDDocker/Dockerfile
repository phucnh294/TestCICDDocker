FROM mcr.microsoft.com/dotnet/framework/aspnet:4.8-windowsservercore-ltsc2022

SHELL ["powershell", "-Command", "$ErrorActionPreference = 'Stop';"]

# Clean default IIS root
RUN Remove-Item -Recurse -Force C:\inetpub\wwwroot\*

# Copy published ASP.NET app
COPY . C:/inetpub/wwwroot/

