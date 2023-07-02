# Flutter Web App SEO Example

This is an example Flutter web application that demonstrates proper SEO (Search Engine Optimization) implementation. It includes meta tags, structured data, and hidden content to improve search engine visibility and provide relevant information to web crawlers.

## Features

- Proper meta tags for title, description, and keywords
- Canonical URL for search engine indexing
- Structured data using JSON-LD format
- Hidden content for SEO purposes

## Getting Started

To run the Flutter web application locally, follow these steps:

1. Clone the repository:
```bash
$ git clone https://github.com/Hemantkumawat/flutter-seo.git
```

2. Install the dependencies:

```bash
$ cd your-repo
$ flutter pub get
```

3. Run the application:
```bash
$ flutter run -d chrome
```

## Implementation Details

### SEOWidget

The `SEOWidget` is a Flutter widget that wraps the content of your application and adds SEO-related metadata. It includes the following attributes:

- `pageTitle`: The title of the page (default: 'MyApp - Your One-Stop Shop for Quick Commerce')
- `pageDescription`: The meta description of the page (default: 'Discover a wide range of products at MyApp. Shop online and enjoy quick and convenient delivery. Start shopping now!')
- `pageKeywords`: The meta keywords of the page (default: 'quick commerce, online shopping, e-commerce, products, delivery')
- `pageUrl`: The canonical URL of the page (default: 'MyApp.com')
- `imageUrl`: The URL of the page's main image (default: 'https://MyApp.com/favicon.png')
- `child`: The child widget that contains the actual content of the page

Note: The `SEOWidget` is only applied if the app is running on a web platform.

### MyApp

The `MyApp` widget is the root of the Flutter application. It includes the `SEOWidget` and sets up the basic structure of the app.

### Usage

To use the `SEOWidget`, simply wrap your content with it. For example, in the `MyHomePage` widget:


```dart
SEOWidget(
    pageTitle: 'Welcome to MyApp',
    pageDescription: 'Discover a wide range of products at MyApp. Shop online and enjoy quick and convenient delivery.',
    child: Center(
        // Your content goes here
    ),
),
```



