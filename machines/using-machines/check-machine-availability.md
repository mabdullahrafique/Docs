# Check availability

## Check machine availability in region

**Usage:** 

```text
gradient machines availability [OPTIONS]
```

Get machine availability for the given region and machine type. Note: availability is only provided for the dedicated GPU machine types. Also, not all machine types are available in all regions.

**Parameters:**

<table>
  <thead>
    <tr>
      <th style="text-align:left"><code>Name</code>
      </th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>region [CA1|NY2|AMS1]</code>
      </td>
      <td style="text-align:left">Name of the region (required)</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><code>machineType [Air|Standard|Pro|Advanced|GPU+|P4000|P5000|</code>
        </p>
        <p><code>P6000|V100|C1|C2|C3|C4|C5|C6|C7|C8|C9|C10]</code>
        </p>
      </td>
      <td style="text-align:left">Machine type (required)</td>
    </tr>
  </tbody>
</table>

**Example usage:**

Command \(example\):

```text
gradient machines availability --region NY2 --machineType P5000 
```

Response \(success\):

`Machine available: True`

Response \(failure\):

`Machine available: False`

 

