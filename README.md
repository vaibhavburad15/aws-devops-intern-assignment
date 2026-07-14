# AWS DevOps Engineer Intern Assignment

## Objective
Deploy a simple website on an AWS EC2 instance using Ubuntu and Nginx.

## Technologies Used

- AWS EC2
- Ubuntu Linux
- Nginx
- Git
- GitHub

## Steps Performed

### 1. Launch EC2 Instance
- Ubuntu Server
- t2.micro
- Security Group with ports:
  - SSH (22)
  - HTTP (80)

### 2. Connect via SSH

```bash
ssh -i aws-devops.pem ubuntu@<EC2_PUBLIC_IP>
```

### 3. Update Packages

```bash
sudo apt update
sudo apt upgrade -y
```

### 4. Install Nginx

```bash
sudo apt install nginx -y
```

### 5. Check Nginx Status

```bash
sudo systemctl status nginx
```

### 6. Restart Nginx

```bash
sudo systemctl restart nginx
```

### 7. Host Website

Created a custom HTML page containing:

- Name
- College
- Branch
- Email
- Current Date

and replaced the default Nginx page.

## Linux Commands Used

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl status nginx
sudo systemctl restart nginx
sudo systemctl enable nginx
df -h
free -h
ps aux
```

## Project Structure

```
aws-devops-intern-assignment/
├── index.html
└── README.md
```

## Author

**Vaibhav Burad**
