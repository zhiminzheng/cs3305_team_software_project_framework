## Development

```bash
# Clone project
git clone https://gitee.com/y_project/RuoYi-Vue

# Enter project directory
cd ruoyi-ui

# Install dependencies
npm install

# It is recommended not to use cnpm directly to install dependencies, as there will be various strange bugs. You can solve the slow npm download speed problem through the following operations
npm install --registry=https://registry.npmmirror.com

# Start service
npm run dev
```

Browser access http://localhost:80

## Release

```bash
# Build test environment
npm run build:stage

# Build production environment
npm run build:prod
```