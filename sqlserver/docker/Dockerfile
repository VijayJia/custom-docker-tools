FROM mcr.microsoft.com/mssql/server:2019-latest AS base
# 接受协议
ENV ACCEPT_EULA=Y

USER root
# 启用SQL Server代理
RUN ["/bin/sh", "/opt/mssql/bin/mssql-conf", "set", "sqlagent.enabled", "true"]

USER mssql