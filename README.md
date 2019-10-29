# post-css

Install post css
```
npm install --save-dev postcss-loader autoprefixer
```
Create postcss.config.js
```
module.exports = {
    plugins: [
      require('autoprefixer')
    ]
  }
```

Add postcss-loader in webpack.config.js file
```
module: {
        rules: [
            {
                test: /\.css$/,
                use: [
                    'style-loader',
                    'css-loader',
                    'postcss-loader'
                ],
            },
        ],
    },
```

