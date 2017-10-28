#### Retrieve all events

##### Arguments

<table>
    <thead>
        <th>Key</th>
        <th>Required</th>
        <th>Type</th>
        <th>Default</th>
        <th>Description</th>
    </thead>
    <tbody>
        <tr>
            <td>$parameters</td>
            <td>false</td>
            <td>array</td>
            <td>null</td>
            <td>Please refer to the list below for a valid list of keys that can be passed on this array.</td>
        </tr>
    </tbody>
</table>

###### $parameters

<table>
    <thead>
        <th>Key</th>
        <th>Required</th>
        <th>Type</th>
        <th>Default</th>
        <th>Description</th>
    </thead>
    <tbody>
        <tr>
            <td>created</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>A filter on the list based on the object created field.</td>
        </tr>
        <tr>
            <td>object_id</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>The object identifier.</td>
        </tr>
        <tr>
            <td>ending_before</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>A cursor to be used in pagination.</td>
        </tr>
        <tr>
            <td>limit</td>
            <td>false</td>
            <td>integer</td>
            <td>10</td>
            <td>A limit on the number of objects to be returned.</td>
        </tr>
        <tr>
            <td>starting_after</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>A cursor to be used in pagination.</td>
        </tr>
        <tr>
            <td>type</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>A string containing a specific event name, or group of events using * as a wildcard.</td>
        </tr>
    </tbody>
</table>

##### Usage

```php
$events = $stripe->events()->all();

foreach ($events['data'] as $event) {
    var_dump($event);
}
```
