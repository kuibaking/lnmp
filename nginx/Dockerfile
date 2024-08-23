FROM nginx:1.24.0

LABEL maintainer="ogenes.yi@gmail.com"

# 复制时区配置
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# 更改权限
RUN mkdir /var/www \
    && chown -R www-data:www-data /var/www/ /var/log/nginx/
