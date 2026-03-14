---
layout: default
title: About
heading: "Clinician-led innovation for surgical excellence"
subheading: "IncisionLabs is a surgical AI and innovation unit based in Singapore, transforming how operating theatres work."
mission_title: "Our Mission"
mission_text: "To provide healthcare professionals with reliable, precision-engineered surgical tools powered by AI that improve patient outcomes and operational efficiency."
vision_title: "Our Vision"
vision_text: "A future where every operating room leverages intelligent systems to deliver safer, more efficient surgical care at scale."
values_title: "Our Values"
values:
  - name: "Clinician-Led"
    description: "Built by surgeons and perioperative specialists who understand frontline realities."
  - name: "Data-Driven"
    description: "Advanced analytics that convert surgical data into actionable intelligence."
  - name: "Systems Thinking"
    description: "Holistic optimization of workflows, not isolated point solutions."
  - name: "Measurable Impact"
    description: "Evidence-based interventions with quantifiable outcomes."
---

<div class="section">
    <div class="page-header reveal">
        <div class="section-label">About Us</div>
        <h1>{{ page.heading }}</h1>
        <p>{{ page.subheading }}</p>
    </div>
</div>

<div class="approach-section">
    <div class="approach-grid">
        <div class="approach-content reveal">
            <h2>{{ page.mission_title }}</h2>
            {{ page.mission_text | markdownify }}
            
            <h2 style="margin-top: 3rem;">{{ page.vision_title }}</h2>
            {{ page.vision_text | markdownify }}
        </div>
        <div class="approach-visual reveal reveal-delay-2">
            {% for value in page.values %}
            <div class="approach-card">
                <div class="card-num">{{ forloop.index | prepend: '0' }}</div>
                <h4>{{ value.name }}</h4>
                <p>{{ value.description }}</p>
            </div>
            {% endfor %}
        </div>
    </div>
</div>

<div class="cta-section">
    <div class="cta-inner reveal">
        <h2>Ready to collaborate?</h2>
        <p>We partner with hospitals and health systems to deploy surgical AI and workflow optimization solutions.</p>
        <a href="{{ '/contact' | relative_url }}" class="btn btn-primary">Contact Us <span class="btn-arrow">&rarr;</span></a>
    </div>
</div>
