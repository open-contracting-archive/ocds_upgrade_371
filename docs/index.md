# Related Process Extension

The related process extension provides a way to link related contracting processes, for example:

* Linking tender processes to pre-qualification or pre-selection processes
* Linking a planning process with the resulting tender processes
* Linking the process to select the parties to a framework agreement with the processes to award procurement processes to such parties.
* Linking unsuccesful or failed tender processes to replacement processes
* Linking sub-contracting processes to parent contracts

Understanding the relationships between contracting processes is important for users to get a full picture of a the contracting process.

The extension introduces a ```relatedProcess``` building block and extends the ```tender``` and ```contract``` sections of OCDS with a new ```relatedProcesses``` field.

## Related Processes Fields

The ```tender/relatedProcesses``` field is an array of ```relatedProcess``` building blocks and can be used to link a processes at the contracting process level, for example linking a PQQ process to an RFP process.

The ```contract/relatedProcesses``` field is an array of ```relatedProcess``` building blocks and can be used to link a contract to it's related processes, for example linking sub-contracting processes to a parent contract.

## Related Process Building Block

The ```relatedProcess``` building block provides a way to:

* State the title and OCID of the related contracting process
* Describe the relationship between the processes using the ```relatedProcess``` codelist
* Link to the URI for the OCDS record of the related contracting process

```eval_rst
.. extensiontable::
   :extension: relatedProcess
```