{ exec } = require 'child_process'

task 'build', 'join and compile *.coffee and *.scss files', ->
  c = exec "node ./node_modules/webpack/bin/webpack --config ./webpack.config.js"
  c.stdout.pipe process.stdout
  c.stderr.pipe process.stderr

task 'watch', 'watch coffee and sass directory for changes and compile', ->
  c = exec "node ./node_modules/webpack/bin/webpack --watch --config ./webpack.config.js"
  c.stdout.pipe process.stdout
  c.stderr.pipe process.stderr
