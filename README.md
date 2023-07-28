# BBM Development Environment

## Github Clone
1. In parent directory, clone from git repository at [BBM Repo](https://github.com/jdrewtopia/bbm.git)
```console
git clone https://github.com/jdrewtopia/bbm.git
```
 **Note** Folder structure will be {parent directory}/bbm

2. In terminal, navigate into bbm directory  
```console
cd bbm
```

## Installation
1. Install dependencies
```console
npm install
```
2. Run application in development mode
```console
npm run dev
```

## Build and Run app for Production
1. Set environment to production
```console
set NODE_ENV=production
```
2. Build then run the app for production
```console
npm run build
npm start
```
**Note** To return to development reset the environment using:
```console
set NODE_ENV=development
```
 

