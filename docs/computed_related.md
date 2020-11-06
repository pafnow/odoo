# Computed / Related Fields

## Computed Field
Computed field is by default readonly and not stored.<br>
It can be stored in the model database table by adding stored=True.<br>
It can be made editable by adding an inverse function.

## Related Field
A related field is by default readonly. It can be made editable by adding readonly=False.<br>
Inverse function is not working on related fields.
