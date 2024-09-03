
2024-09-01 21:20

### Overview
Joi is a validation schema.

### Basic setup
```javascript
import Joi from 'joi';

const schema = Joi.object().keys({
    name: Joi.string().alphanum().min(3).max(30).required(),
    birthyear: Joi.number().integer().min(1930).max(2013),
})

const dataToValidate = {
    name: 'chris',
    birthyear: 1971
}

const result = Joi.validate(dataToValidate, schema);
```

### References
- [[Interview Prep]]

