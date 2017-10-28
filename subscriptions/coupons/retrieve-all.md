#### Retrieve all coupons

Returns a list of your coupons.

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
            <td>customer</td>
            <td>false</td>
            <td>string</td>
            <td>null</td>
            <td>The customer unique identifier.</td>
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
    </tbody>
</table>

##### Usage

```php
$coupons = $stripe->coupons()->all();

foreach ($coupons['data'] as $coupon) {
    var_dump($coupon['id']);
}
```
