
### add gem config
```
gem 'sunspot_rails'
gem 'sunspot_solr' # optional pre-packaged Solr distribution for use in development
```
### install gem 
```
bundle
```

## install config
```
rails generate sunspot_rails:install
```
### 
```
bundle exec rake sunspot:solr:start # or sunspot:solr:run to start in foreground
```
###
```
rake sunspot:reindex
```
