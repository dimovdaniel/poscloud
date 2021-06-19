# Import from CSV

## Enable importing restaurants from Excel

As usual way of adding manually restaurants this platform has option for adding restaurants from excel files. 

To enable this option you need to add the **ENABLE\_IMPORT\_CSV** variable in **env** file with **true** value.

If you want to disable this option you need to add **false** value.

```
ENABLE_IMPORT_CSV=true
```

{% hint style="info" %}
 Only admin users have access to this option.
{% endhint %}

### Excel file data format

This option has predefined format of the excel file for importing the data. Any other format can cause unwanted import of the data.

| name | description | address | restaurant phone | logo | owner email | owner name | owner password | owner phone |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|  |  |  |  |  |  |  |  |  |

{% file src="../.gitbook/assets/restaurants \(2\).csv" caption="Example restaurants csv file" %}

## Enable importing restaurant items from Excel

As usual way of adding manually restaurant items this platform has option for adding restaurant items from excel files. 

To enable this option you need to add the **ENABLE\_IMPORT\_CSV** variable in **env** file with **true** value.

If you want to disable this option you need to add **false** value.

```
ENABLE_IMPORT_CSV=true
```

{% hint style="info" %}
Only admin and restaurant owner have access to this option. 
{% endhint %}

## Excel file data format

This option has predefined format of the excel file for importing the data. Any other format can cause unwanted import of the data.

| name | description | price | category | image |
| :--- | :--- | :--- | :--- | :--- |
|  |  |  |  |  |

{% file src="../.gitbook/assets/items \(2\).csv" caption="Example items csv file" %}

