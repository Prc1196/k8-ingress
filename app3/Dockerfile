FROM nginx
RUN rm -rf /usr/share/nginx/html/index.html
#RUN echo "<h1> Hello , I am  from app-3</h1>" > /usr/share/nginx/html/index.html


# Create a new HTML page that includes an image
RUN echo '\
<html>\
  <body>\
    <h1>Hello, I am from app-3</h1>\
    <img src="dockerimage.jpg" alt="Sample Image" width="300"/>\
  </body>\
</html>' > /usr/share/nginx/html/index.html

# Copy the actual image file into the container
COPY dockerimage.jpg /usr/share/nginx/html/