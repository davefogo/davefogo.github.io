A great method I found online is the each_slice. I searched for a long while on how to set 3 columns of my objects in the index page. At the beginning I thought this was only possible through css styling. It turns out you can do it with ruby. This awesome loop construct takes your array and “slices it” into groups of n units. When mixed with row CSS styling you can give your lists a new look. This is particularly useful when trying to display various columns in an index page.

Example: 

```
@list = [ "apple", "banana", "coconut", "durian", "eggfruit", "fig", "grapefruit", "honeydew", "Ita Palm", "jujube", "kiwi", "lime", "mango"]
<div class="row">
  @list.each_slice(3) do |lists| 
    <% lists.each do |item| %>
      <div class="col-sm-4>
        <%= item %>
    <% end %>
  <% end %>
</div>
```
