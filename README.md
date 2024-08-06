# THINGS IN HERE

## GEMS

```
gem 'devise'
```
- devise set for turbo, rails 7
- from: https://dev.to/efocoder/how-to-use-devise-with-turbo-in-rails-7-9n9

## MODELS
- devise user
- posts scaffold
- comment belongs to post added to a do block in routes, with posts
- validations for posts

```
  validates :title, presence: true, length: {minimum: 5}
  validates :body,  presence: true
```

## OTHER
- he did his own styling
- used normalize.css
- added favicon
- added a 'mailto' link
- did an svg logo
- image in the about page
- if current_page?

```
      <% if current_page?(root_path) %>
        <p>All Posts</p>
      <% elsif current_page?(about_path) %>
        <p>About</p>
      <% else %>
        <%= link_to "Back to All Posts", root_path %>
      <% end %>
```