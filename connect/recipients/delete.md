#### Delete a recipient

Permanently deletes a recipient. It cannot be undone.

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
            <td>$recipientId</td>
            <td>true</td>
            <td>string</td>
            <td>null</td>
            <td>The recipient unique identifier.</td>
        </tr>
        <tr>
            <td>$cardId</td>
            <td>true</td>
            <td>string</td>
            <td>null</td>
            <td>The card unique identifier.</td>
        </tr>
    </tbody>
</table>

##### Usage

```php
$recipient = $stripe->recipients()->destroy([
    'id' => 'rp_4EYRyEYthf2Doc',
]);
```
