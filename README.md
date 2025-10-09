# 🧁 Candy Spark
A fun, colorful, and responsive match-3 candy game built with HTML, CSS, and JavaScript — inspired by the mechanics of Candy Crush but with unique features like a 2-minute timer, score tracker, and special candies that create chain reactions!
 🎮 Made just for fun — match, swap, and spark your way to the highest score!

 
 # 🐳 Docker Hosting Steps
You can easily containerize and run this project with Docker.
Follow these steps exactly 👇

## 1️⃣ Create a Dockerfile
In your project folder (where index.html is located), create a file named Dockerfile and add this code:
<pre>```
# Use official Nginx image as base
FROM nginx:alpine

# Copy all project files to Nginx default HTML directory (HTML/CSS/JAVASCRIPT)
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx server
CMD ["nginx", "-g", "daemon off;"]
 ```</pre>

## 2️⃣ Build the Docker Image
Open your terminal in the project folder and run:
<pre>``docker build -t candy-spark-game .
 ```</pre>

 ## 3️⃣ Run the Docker Container
 <pre>```docker run -d -p 8080:80 --name candy-spark candy-spark-game
```</pre>

Now open your browser and go to:
👉 [Link Text](http://localhost:8080)
You’ll see Candy Spark running inside a container 🚀

# 📸 Screenshot
![Candy Spark Screenshot](screenshot.png)


