# Feedback For Restaurant Customer Service

Professional template for gathering customer feedback in the hospitality industry, focusing on restaurant service.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Hospitality
- **Message Type:** Feedback
- **Tags:** customer service, restaurant feedback

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/feedback-for-restaurant-customer-service.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/feedback-for-restaurant-customer-service/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.feedback-for-restaurant-customer-service',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
