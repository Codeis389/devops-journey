# DevOps Concepts - What is What?

## What is Nginx?
Nginx is a web server software.
- It serves your HTML/CSS/JS files to users
- When someone opens your website, nginx sends the files
- Also used as reverse proxy and load balancer
- Userd by: Netflix, Dropbox, WordPress
- Think of it as: a waiter that delivers your website to visitors.

## What is Kubernetes?
Kubernetes is a container management system.
- Docker runs ONE container
- Kubernetes manages HUNDREDS of containers
- Auto restarts crashed containers (self healing)
- Auto scales when traffic increases
- Used by: Google, Netflix, Spotfy, NASA
- Think of it as: a manager that controls all your Docker containers

## What is Docker?
Docker is a conainerization tool.
- Packages your app + everything it needs into one box
- Works the same on any computer or server
- No more "works on my machine" problem
- Think of it as: a shipping continer for your app.

## What is a POD?
smallest unit in Kubernetes.
- Holds one or more containers
- Like a wrapper around your Docker container
- Think of it as: a box that holds your container

## What is a Node?
A server/machine in Kubernetes cluster.
- Runs your pods
- can be physical or cloud server
- Think of it as: a worker that runds your apps

## What is a Cluster?
A group of nodes working together.
- Multiple servers managed as one
- Think of it as: a team of workers

## What is a Deployment?
Tells Kubernetes how to run your app.
- How many copies to run (replicas)
- Which image to use
- Auto restarts if pod crashes
- Think of it as: instructions for running your app.

## What is a Service?
Exposes your app to the internet.
- Without service = app is hidden inside cluster.
- with service = app is accessible viw URL
- Think of it as: a door to your app

## What is CI/CD?
Continuous Integration / Continuous Deployment
- CI = automatically test your code on every push
- CD = automatically deploy your codeon every push
- No manual work needed
- Think of it as: auto pilot for your code

## What is GitHub Actions?
CI/CD tool built inot GitHub.
- Runs automatically when you push code
- Can test, build, and deploy your app
- Free for public repostories
- Think of it as: a robot that deploys your code

## What is Netlify?
A cloud platform for deploying websites.
- Connect GitHub repo - auto deploys on every push
- Free tier available
- Gives you a public URL instantly
- Think of it as: magic website hosting

## What is BAsh Scripting?
Writign commands in a file to automate tasks.
- Instead of typing commands one by one.
- Write them in a file and run once
- Rreal DevOps automation tool
- Think of it as: a recipe of commands

## What is SSH?
Source Shell - remote server access.
- Connect to servers from anywhere
- Like remote control for servers
- Used to manage cloud servers.
- Think of it as: a secure tunnel to your server.

## What is Linux?
Operating system used by 90% of servers.
- Free and opne source
- More stable and secure than Windows
- Every DeoOps engineer must know Linux
- Think of it as: the engine that runs the internet 

# Day 6 - Kubernetes (K8s)

## Installation

- kubectl = Controls kubernetes
- minikube = kubernetes on local machine
- minikube start --driver=docker = start cluster
- minikube stop = stop cluster
- minkube status = check status

## Basic Commands

- kubectl get nodes = see all nodes
- kubectl get pods = see all pods
- kubectl get services = see all services
- kubectl get all = see everything

## Deploy App

- kubectl create deployment myapp --image=nginx
- kubectl expose deployment myapp --port=80 --type=NodePort
- minikube service myapp --url = get app URL

## Cleanup

- kubectl delete deployment myapp
- kubectl delete service myapp
- minikube stop

## Key Concepts

- Pod = smallest unit (holds container)
- Node = server running pods
- Cluster = group of nodes
- Deployment = manages pods
- Service = expose app to internet
- Self Healing = K8s auto restarts crashed pods!
