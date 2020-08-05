# Odoo development
This note will summarize key concepts for Odoo development.

## Inheritance
Odoo's programming is based on the concept of inheritance: each feature consists in a module creating its own objects and modifying existing one via inheritance. Inheritance can be made on several type of objects depending on the need.

### Models
- [Official Documentation](https://www.odoo.com/documentation/13.0/reference/orm.html#inheritance-and-extension)
```python
from odoo import api, fields, models

class ResPartner(models.Model):
    _inherit = 'res.partner'

    test_payment_term_id = fields.Many2one('account.payment.term', company_dependent=False, 
        string='Test Customer Payment Terms',
        help="Test This payment term will be used instead of the default one for sales orders and customer invoices")
```

### Controllers
- [Official Documentation](https://www.odoo.com/documentation/13.0/reference/http.html#controllers)

### Views
- [Official Documentation](https://www.odoo.com/documentation/13.0/reference/views.html#inheritance)

### Javascript
- [Official Cheatsheet](https://www.odoo.com/documentation/13.0/reference/javascript_cheatsheet.html#modifying-an-existing-field-widget)
- [Official Documentation](https://www.odoo.com/documentation/13.0/reference/javascript_reference.html#inheritance)

## Debugging
During the development phase, it is often needed to do some debugging / logging in order to understand the logic of the application. Similar to inheritance, logging is different for each type of objects used.

### Models

### Controllers

### Views

### Javascript
