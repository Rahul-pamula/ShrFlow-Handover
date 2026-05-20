---
title: 'Introduction'
description: 'The high-performance email delivery engine for modern software teams.'
icon: 'book-open'
---

ShrFlow is an enterprise-grade email infrastructure platform. Built on top of Next.js, FastAPI, RabbitMQ, and Supabase, it provides unparalleled performance for managing audiences, designing templates, and dispatching multi-million-contact email campaigns.

![ShrFlow Dashboard](screen-shots/dashboard.png)

<div class="card-grid">
  <a class="card" href="#/getting-started/quick-start">
    <h4><span>⚡</span> Quick Start</h4>
    <p>Launch your first campaign and verify your developer cluster in under 10 minutes.</p>
  </a>
  <a class="card" href="#/api-reference/authentication">
    <h4><span>🔑</span> API Reference</h4>
    <p>Integrate ShrFlow programmatically into your client products using REST APIs.</p>
  </a>
  <a class="card" href="#/advanced/deliverability-engine">
    <h4><span>⚙️</span> Engine Architecture</h4>
    <p>Understand the low-latency dual-delivery queue and deliverability performance routing.</p>
  </a>
  <a class="card" href="#/advanced/webhooks">
    <h4><span>🔗</span> Real-time Webhooks</h4>
    <p>Stream real-time email dispatch, click, and bounce tracking events.</p>
  </a>
</div>

## System Architecture

ShrFlow is designed to be fully containerized, stateless at the edge, and highly available. It relies on horizontal scaling and message brokers to guarantee email delivery under intense load without dropping packets.
