
### add gem config
```
gem 'sunspot_rails'
gem 'sunspot_solr' # optional pre-packaged Solr distribution for use in development
```
### install gem 
```
bundle
```

### install config
```
rails generate sunspot_rails:install
```
### start sunspot engine
```
bundle exec rake sunspot:solr:start # or sunspot:solr:run to start in foreground
```

### add what field you want to make it searchable
```
class Site < ApplicationRecord

  # sunspot gem
  searchable do
    text :name, :url, :description
  end
  
end
```
### make index
```
rake sunspot:reindex
```

### add html
```
<%= form_tag articles_path, :method => :get do %>
  <p>
    <%= text_field_tag :search, params[:search] %>
    <%= submit_tag "Search", :name => nil %>
  </p>
<% end %>
```
