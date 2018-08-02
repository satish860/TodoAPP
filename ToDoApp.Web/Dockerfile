# escape=`
FROM microsoft/aspnet:4.7.2-windowsservercore-ltsc2016
WORKDIR C:\web-app
RUN Remove-Website -Name 'Default Web Site'; `
    New-Website -Name 'web-app' -Port 80 -PhysicalPath 'C:\web-app'
EXPOSE 80
COPY "/bin/release/publish/" .
