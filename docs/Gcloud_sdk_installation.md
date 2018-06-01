## **1. How to install GCloud SDK in local shell?**
#### Tutorial https://cloud.google.com/sdk/

### Try Mac OS and Unix Interactive installer
#### 1) Enter the following at a command prompt:
```markdown
curl https://sdk.cloud.google.com | bash
```
#### 2) Restart your shell:
```markdown
exec -l $SHELL
```

#### 3) Run gcloud init to initialize the gcloud environment:
```markdown
gcloud init
```

## **2. How to authorize gcloud?**
#### Go to https://cloud.google.com/ click "Try it free" if you don't have an account
#### Register with your email account, e.g. youremail@address.com
#### Authorize gcloud in your local shell:
```markdown
gcloud auth login
```

## **3. How to create and set a project?**
#### A Project resource is required to use GCP and forms the basis for using GCP services, enabling billing and etc.
#### Tutorial https://cloud.google.com/sdk/gcloud/reference/projects/

#### 1) Create a new cloud PROJECT_ID console.developers.google.com
#### or create a mew cloud project_ID in local shell:
```markdown
gcloud projects create 
```
#### 2) Set a project in local shell:
```markdown
gcloud config set account youremail@address.com
gcloud config set project PROJECT_ID
```

## **4. How to install gcloud alpha interactive in local shell?**
#### Tutorial https://cloudplatform.googleblog.com/2018/03/introducing-GCPs-new-interactive-CLI.html
#### 1) Update SDK components:
```markdown
gcloud components update
```
#### 2) Install the gcloud alpha component:
```markdown
gcloud components install alpha
```
#### 3) Start gcloud interactive:
```markdown
gcloud alpha interactive
```
#### 4) exit the interative shell by F9 or:
```markdown
exit
```
