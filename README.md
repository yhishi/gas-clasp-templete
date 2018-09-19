# gas-clasp-templete

## Getting Started
### Clone the repository
```
git clone --depth=1 https://github.com/yhishi/gas-clasp-templete.git <project_name>
```

### Install dependencies
```
cd <project_name>
npm install
```

### Configuration
##### Open `.clasp.json`, change scriptId
What is scriptId ? https://github.com/google/clasp#scriptid-required
```
{
  "scriptId": <your_script_id>,
  "rootDir": "dist"
}
```

### Development and build project
```
npm run build
```

### Push
```
clasp push
```

### Error `shallow update not allowed` Soulution
```
git remote add old https://github.com/yhishi/gas-clasp-templete
git fetch --unshallow old
```
By doing so you can push as usual.