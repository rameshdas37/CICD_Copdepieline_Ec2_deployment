Architecture (Simple & Practical)

GitHub / CodeCommit
        |
        v
   CodePipeline
        |
        v
   CodeBuild
   (Build + Test)
        |
        v
   CodeDeploy
   (Deploy to EC2)
We will deploy a Python Flask app to EC2.

Project structure (important)
my-flask-app/
├── app.py
├── requirements.txt
├── buildspec.yml
├── appspec.yml
└── scripts/
    ├── install_dependencies.sh
    ├── start_server.sh
    └── stop_server.sh
Step 1 – Create EC2 Instance (Deployment Target)
EC2 Setup
Launch Amazon Linux 2
Attach IAM Role:
AmazonEC2RoleforAWSCodeDeploy
Install CodeDeploy Agent:
