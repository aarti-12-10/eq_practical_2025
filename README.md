# Shopify Take Home Assignment

## Overview

- We need to develop a Shopify site using the provided Figma design file and Dawn as the base theme. The focus should be on creating a fully functional home page with the specified features.
- You will be invited to a development Shopify store using your email ID.
- The Shopify store will already be populated with dummy data.
- Create a copy of the live theme and make changes in a new theme using your name as the theme name with appropriate naming convention.

## Figma Link

[Figma Design](https://www.figma.com/file/1EFMnOIJo1zTamuOUE2kOO/eQuest-Solutions---UI-Practical?type=design&node-id=0%3A1&mode=design&t=EpYbl9bJZ2gOLKA2-1)

## Requirements

### Base Theme

- **Dawn Theme**: Use Dawn as the base theme for the development.

### Home Page

- **Product with Options and Variants**:
  - The product section should show a product with the size and color option and on selection the image should change to that color.
- **Upsell Offer**:
  - When the product is added to the cart, an additional free item should also be added automatically.
  - The quantity of the free item should match the quantity of the paid item.
  - The selection of the free item should be configurable at the product level in the admin panel.
- **AJAX Add to Cart**:
  - Use AJAX for the 'Add to Cart' functionality.
  - Reference: [Shopify AJAX API - Cart](https://shopify.dev/docs/api/ajax/reference/cart)

### Predictive Search

- Implement predictive search functionality.
- Reference: [Shopify Predictive Search API](https://shopify.dev/docs/api/ajax/reference/predictive-search)

### Checkout

- **Auto-apply Discount**:
  - A discount of value 10 should be automatically applied when proceeding to checkout.
  - This discount should be in addition to the free items being added.

## Advanced Features

### Shopify Markets

- **Multi-Market Setup**:
  - Configure at least 2 different markets (e.g., US and Canada).
  - Set up different pricing for each market using market-specific pricing.
  - Implement currency conversion and display appropriate currency symbols.
  - Configure different shipping zones and rates for each market.
- **Market Selection**:
  - Add a market/country selector in the header or footer.
  - Ensure the selector updates pricing, currency, and shipping information dynamically.
  - Store the selected market in the customer's session.
- **Localization**:
  - Implement basic localization for at least one non-English market.
  - Translate key product information and UI elements.

### Metaobjects

- **Custom Data Structure**:
  - Create a metaobject definition for "Product Specifications" with fields like:
    - Material (single line text)
    - Dimensions (single line text)
    - Weight (number)
    - Care Instructions (multi-line text)
    - Warranty Period (single line text)
- **Product Integration**:
  - Create a metafield on products that references the Product Specifications metaobject.
  - Display the specification data on the product page in a well-formatted section.
  - Ensure the data is easily manageable from the Shopify admin.
- **Dynamic Content**:
  - Use the metaobject data to create dynamic content sections.
  - Implement conditional rendering based on metaobject field values.

### Shopify Flow Automation

- **Inventory Management Flow**:
  - Create a Flow that triggers when product inventory falls below 5 units.
  - Set up an action to tag the product as "Low Stock".
  - Configure an email notification to be sent to the store admin.
- **Customer Segmentation Flow**:
  - Create a Flow that triggers when a customer places their first order.
  - Add the customer to a "First Time Buyers" segment.
  - Set up a follow-up email sequence (if email capabilities are available).
- **Order Processing Flow**:
  - Create a Flow that triggers when an order contains a high-value item (over $100).
  - Add a tag to the order for "High Value Order".
  - Set up a notification to prioritize fulfillment.
- **Flow Documentation**:
  - Document each Flow's purpose, triggers, conditions, and actions.
  - Include screenshots of the Flow setup in your documentation.

## Technical Implementation Guidelines

### Code Structure

- **Liquid Templates**: Follow Shopify's best practices for Liquid templating.
- **JavaScript**: Use modern ES6+ JavaScript and ensure cross-browser compatibility.
- **CSS**: Maintain the Bootstrap styling while ensuring responsiveness.
- **Performance**: Optimize for Core Web Vitals and page load speed.

### Testing Requirements

- **Cross-Market Testing**: Verify functionality across different markets and currencies.
- **Metaobject Testing**: Ensure metaobject data displays correctly and handles missing data gracefully.
- **Flow Testing**: Test all Flow triggers and verify actions execute as expected.
- **Mobile Responsiveness**: Ensure all features work seamlessly on mobile devices.
- **Browser Compatibility**: Test across Chrome, Firefox, Safari, and Edge.

### Development Workflow

- **GitHub Commits**:
  - Commit changes to GitHub after completing each page or significant feature.
  - Ensure commits are clear and concise, detailing what has been implemented.
  - Use descriptive commit messages following conventional commit format.
- **Branch Strategy**:
  - Create separate branches for major features (e.g., `feature/markets`, `feature/metaobjects`, `feature/flows`).
  - Merge branches via pull requests with proper documentation.
- **Documentation**:
  - Create a comprehensive README documenting setup instructions.
  - Include screenshots of admin configurations for Markets, Metaobjects, and Flows.
  - Document any custom liquid filters or JavaScript functions created.

## Deliverables

### Core Requirements
1. **Template & Theme**: Figma design developed with Dawn theme as the base theme.
2. **Home Page**: Product section, upsell offers, AJAX cart, related products.
3. **Search**: Predictive search functionality.
4. **Checkout**: Auto-applied discount functionality.

### Advanced Requirements
6. **Markets**: Multi-market setup with currency/pricing configuration.
7. **Metaobjects**: Custom product specifications with dynamic display.
8. **Flows**: Three automated workflows with proper documentation.

### Documentation
9. **Setup Guide**: Step-by-step instructions for reproducing the setup.
10. **Feature Documentation**: Detailed explanation of each implemented feature.
11. **Admin Screenshots**: Visual documentation of admin configurations.

## Evaluation Criteria

- **Code Quality**: Clean, maintainable, and well-commented code.
- **Feature Implementation**: All requirements met with proper functionality.
- **User Experience**: Intuitive and responsive design implementation.
- **Technical Depth**: Understanding of advanced Shopify concepts.
- **Documentation**: Clear and comprehensive documentation.
- **Problem Solving**: Creative solutions to technical challenges.

Please follow the instructions carefully and ensure each feature is thoroughly tested before committing to GitHub. Document any challenges faced and solutions implemented. If you have any questions or need further clarifications, feel free to reach out.
