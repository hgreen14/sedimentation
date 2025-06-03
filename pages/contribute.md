---
title: Share Your Sediment Story
layout: page
permalink: /contribute/
---

# Share Your Sediment Story

The sediment that flows through our rivers and shapes our landscapes carries countless stories. We invite you to contribute your own experiences, knowledge, and perspectives about sediment to this growing collection.

## How to Contribute

### Submit a Story
Have you witnessed a dramatic erosion event? Observed changes in your local river over time? Experienced flooding that changed your landscape? Share your story with us.

<div class="card mt-4 mb-4">
<div class="card-body">
<h5 class="card-title">Story Submission Form</h5>
<form id="story-form" class="needs-validation" novalidate>
  <div class="row">
    <div class="col-md-6 mb-3">
      <label for="story-title" class="form-label">Story Title *</label>
      <input type="text" class="form-control" id="story-title" required>
      <div class="invalid-feedback">Please provide a title for your story.</div>
    </div>
    <div class="col-md-6 mb-3">
      <label for="story-location" class="form-label">Location</label>
      <input type="text" class="form-control" id="story-location" placeholder="City, State/Province, Country">
    </div>
  </div>
  
  <div class="row">
    <div class="col-md-6 mb-3">
      <label for="story-author" class="form-label">Your Name *</label>
      <input type="text" class="form-control" id="story-author" required>
      <div class="invalid-feedback">Please provide your name.</div>
    </div>
    <div class="col-md-6 mb-3">
      <label for="story-email" class="form-label">Email Address *</label>
      <input type="email" class="form-control" id="story-email" required>
      <div class="invalid-feedback">Please provide a valid email address.</div>
    </div>
  </div>
  
  <div class="mb-3">
    <label for="story-category" class="form-label">Story Category</label>
    <select class="form-select" id="story-category">
      <option value="">Select a category...</option>
      <option value="formation">Formation & Erosion</option>
      <option value="movement">Sediment Movement</option>
      <option value="accumulation">Accumulation & Deposition</option>
      <option value="ecosystem">Ecosystem Impact</option>
      <option value="infrastructure">Infrastructure & Engineering</option>
      <option value="indigenous">Indigenous Knowledge</option>
      <option value="future">Future Visions</option>
      <option value="other">Other</option>
    </select>
  </div>
  
  <div class="mb-3">
    <label for="story-content" class="form-label">Your Story *</label>
    <textarea class="form-control" id="story-content" rows="6" required 
              placeholder="Tell us your sediment story. What did you observe? How did it impact you or your community? What insights did you gain?"></textarea>
    <div class="invalid-feedback">Please share your story.</div>
  </div>
  
  <div class="mb-3">
    <label for="story-date" class="form-label">When did this occur?</label>
    <input type="date" class="form-control" id="story-date">
  </div>
  
  <div class="mb-3">
    <label for="story-images" class="form-label">Images (optional)</label>
    <input type="file" class="form-control" id="story-images" multiple accept="image/*">
    <div class="form-text">You can upload multiple images. Please ensure you have permission to share these images.</div>
  </div>
  
  <div class="form-check mb-3">
    <input class="form-check-input" type="checkbox" id="story-consent" required>
    <label class="form-check-label" for="story-consent">
      I consent to having my story included in this public collection and understand that it may be used for educational and research purposes. *
    </label>
    <div class="invalid-feedback">Please provide your consent.</div>
  </div>
  
  <button type="submit" class="btn btn-primary btn-lg">Submit Story</button>
</form>
</div>
</div>

### Contribute Research or Data

Are you a researcher, student, or professional working with sediment data? We welcome contributions of:

- Research findings and publications
- Data sets and measurements
- Historical photographs and documentation
- Maps and visualizations
- Educational resources

<div class="alert alert-info mt-3">
<strong>Research Contribution:</strong> Please email us at <a href="mailto:contribute@sedimentation.org">contribute@sedimentation.org</a> with details about your research or data contribution.
</div>

### Community Knowledge

Traditional and local knowledge about sediment systems is invaluable. We especially welcome:

- Traditional ecological knowledge
- Long-term observations from community members
- Stories from Indigenous communities
- Historical accounts from local residents
- Intergenerational knowledge about landscape changes

## Submission Guidelines

### What We're Looking For

- **Personal experiences** with sediment, erosion, or river changes
- **Observations** of environmental changes over time
- **Traditional knowledge** about sediment cycles and management
- **Professional insights** from relevant fields
- **Community impacts** of sediment-related events
- **Creative expressions** inspired by sediment and rivers

### Content Standards

- Stories should be truthful and based on real experiences
- Please respect privacy and get permission before sharing others' stories
- Images should be your own or used with permission
- Content should be appropriate for all audiences
- We welcome diverse perspectives and voices

### Privacy and Attribution

- Your name will be associated with your contribution unless you request otherwise
- Email addresses will not be made public
- We may contact you for clarification or follow-up
- You retain ownership of your submitted content
- Stories become part of the public educational collection

## What Happens Next

1. **Review Process**: Submitted stories are reviewed for appropriateness and accuracy
2. **Integration**: Approved stories are integrated into the collection with proper attribution
3. **Connection**: Stories may be connected to relevant geographical locations or themes
4. **Sharing**: Your story becomes part of the growing sediment narrative collection

## Contact Us

Have questions about contributing? Want to discuss a large contribution or partnership?

**Email**: [contribute@sedimentation.org](mailto:contribute@sedimentation.org)

**Mailing Address**:
Sedimentation Stories Project
[Address to be added]

---

*Thank you for helping us build a comprehensive understanding of how sediment shapes our world and our lives. Every story matters in creating the full picture of our relationship with these dynamic earth systems.*

<script>
// Form validation and submission
(function() {
  'use strict';
  
  // Add form validation
  const form = document.getElementById('story-form');
  
  form.addEventListener('submit', function(event) {
    if (!form.checkValidity()) {
      event.preventDefault();
      event.stopPropagation();
    } else {
      event.preventDefault();
      // Here you would normally submit to a server
      // For now, just show a thank you message
      showThankYou();
    }
    
    form.classList.add('was-validated');
  });
  
  function showThankYou() {
    const formContainer = document.querySelector('#story-form').parentElement;
    formContainer.innerHTML = `
      <div class="alert alert-success" role="alert">
        <h4 class="alert-heading">Thank you!</h4>
        <p>Your story has been submitted successfully. We'll review it and be in touch soon.</p>
        <hr>
        <p class="mb-0">Your contribution helps build our understanding of sediment systems and their impact on communities worldwide.</p>
      </div>
    `;
  }
})();
</script>
