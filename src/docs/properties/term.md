---
title: Term
type: properties
---

```php
<?php

/**
 * Example of term.
 */

papi_property( [
  'title'    => 'Term',
  'slug'     => 'my_term_slug',
  'type'     => 'term',
  'settings  => [
    'taxonomy' => 'my_taxonomy'
  ]
] )

/**
 * Example output.
 */

stdClass Object
(
    [term_id] => '123'
    [name] => 'The term'
    [slug] => 'the_term'
    [term_group] => '0'
    [term_order] => '0'
    [term_taxonomy_id] => '321'
    [taxonomy] => 'my_taxonomy'
    [description] => ''
    [parent] => '0'
    [count] => '0'
    [object_id] => ''
)
```

### Description

With this property you can add reference to a term in a taxonomy. It can't handle multiple terms or taxonomies.

### Settings

Key           | Default       | Description
--------------|---------------|--------------------------------------------------
placeholder   | null          | Placeholder text that's displayed when no option is slected.
taxonomy      | 'post'        | The taxonomy that the property will load terms from. Can only be one taxonomy.
select2       | true          | If true Select2 will be used, if false the native browser dropdown will be used.
query         | array         | Add `get_terms` arguments.
