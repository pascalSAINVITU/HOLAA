# HOLLAA
Holder of Linked Lists AA
HOLLAA makes it easier to manipulate small linked lists

## use cases / input fields associations
### create, add and remove
* Add item to a list: 'list_name = <list name>', 'add = <item name>', optionaly 'value = <value, or true by default>';
* Remove item by name: 'list_name = <list name>', 'remove = <item name>';
* Insert before existing item = 'list_name = <list name>', 'insert = <item name>', optionaly 'value = <value, or true by default>' and 'before = <existing item name>' or 'after = <existing item name>';
* Delete existing list: 'list_name = <list name>', 'delete' = true;

### Get item with trigger
* Get next as a trigger: 'list_name = <list name>', 'get_next = <actual item name>'. You will received 4 bytes payment with data.item_key and data.item_value;
* Get previous as a trigger: 'list_name = <list name>', 'get_previous = <actual item name>'. You will received 4 bytes payment with data.item_key and data.item_value;

### access item from state
* Access item by name: var[$HOLLAA_ADDRESS][$list_name||"_"||$item_name];
* Access first element: var[$HOLLAA_ADDRESS][$list_name||"_first_item"];
* Access next element: var[$HOLLAA_ADDRESS][var[$HOLLAA_ADDRESS][$list_name||"_"||$item_name]||"_next_item"];
* Access last element: var[$HOLLAA_ADDRESS][$list_name||"_last_item"];
* Access previous element: var[$HOLLAA_ADDRESS][var[$HOLLAA_ADDRESS][$list_name||"_"||$item_name]||"_previous_item"];
