2}

create folder travel-agency
add index.html

  //   Dockerfile:-

              # Use official nginx image to serve static files
FROM nginx:stable-alpine

# Remove default nginx content
RUN rm -rf /usr/share/nginx/html/*

# Copy site content into nginx's serving directory
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start nginx in foreground (default command)
CMD ["nginx", "-g", "daemon off;"]


 //    .dockerfile:-
     
     .git
node_modules
*.log

// terminal copy paste

 git init
>> git add .
>> git commit -m "Initial commit: two-page travel site"
>>
>> 
>>  git remote add origin https://github.com/Vishal4363/tr.git           // add repository copy//          
>> git branch -M main
>> git push -u origin main
>
>
>docker build -t travel-agency:1.0 .
>
>docker images
>docker rm -f travel-site
>docker build -t travel-agency .
>docker run -d --name travel-site -p 8081:80 travel-agency

     
