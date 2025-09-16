# Use the official Nginx image as base
FROM nginx:alpine

# Remove the default nginx static files
RUN rm -rf /usr/share/nginx/html/*

# Clone the website repository
RUN git clone git@github.com:hashtechinfosystems/htis-web.git

# Copy your HTML and images to the nginx web root
COPY htis-web/webapp/* /usr/share/nginx/html/

# Expose port 80
EXPOSE 80
