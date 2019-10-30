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

# cssNano
Install cssNano
```
npm install cssnano --save-dev
```
Add plugins to post.config.js file
```
module.exports = {
    plugins: [
      require('autoprefixer'),
      require('cssnano')({
          preset: 'default',
      }),
    ],
  }
```
