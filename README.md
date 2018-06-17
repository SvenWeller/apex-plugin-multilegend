# apex-plugin-multilegend
Legend with multiple sections
The legend plugin takes a SQL data source in the form 
<pre>
  select 'section'      as title,
         'name'         as text,
         '1 name'       as category,
         'Filter: name' as shortDesc,
         null           as color
    from myTable
</pre>

A legend can consist of several sections. 
The title is the section title, and each text entry will be the named entry inside this legend section.
Multiple different sections can be added to a single legend.
If there is the same text inside multiple sections, for example UNKNOWN. Then the category needs to be made unique.

Categories are used to connect a JET legend with a JET chart. If no category is set, then the text column is used.
