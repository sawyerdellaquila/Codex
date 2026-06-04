# Dell'Aquila Performance Group Shop Management Software — Product Requirements Document v1.0

## Document Control

| Field | Value |
| --- | --- |
| Product | Dell'Aquila Performance Group Shop Management Software |
| Document type | Product Requirements Document (PRD) |
| Version | 1.0 |
| Prepared for | Dell'Aquila Performance Group |
| Target business | Porsche/BMW European performance automotive shop |
| Target launch context | Sacramento-area performance shop planned for early next year |
| Status | Draft for review |

## 1. Executive Summary

Dell'Aquila Performance Group needs a modern automotive shop management platform tailored to the realities of a Porsche/BMW European performance shop. The system should improve on legacy shop systems such as MaxxTraxx/MaxTracks while matching or exceeding the usability expectations set by newer platforms such as Shopmonkey.

The product should support daily shop operations including customer management, vehicle records, estimates, repair orders, scheduling, technician workflow, parts tracking, invoicing, payments, and reporting. It should also support performance-shop-specific workflows such as modification history, build profiles, track preparation, alignment specifications, dyno results, tuning references, and reusable Porsche/BMW service packages.

The recommended strategy is to build a practical MVP for operating Dell'Aquila Performance Group first, then expand into advanced workflow, parts, inventory, analytics, and performance-build capabilities after the core shop flow is validated.

## 2. Product Vision

Create a fast, modern, technician-friendly, advisor-friendly shop management system that gives Dell'Aquila Performance Group a competitive operational advantage. The product should reduce administrative work, improve customer communication, increase estimate approval rates, organize vehicle and build history, and provide clear visibility into shop workload and profitability.

The software should feel purpose-built for a specialty performance shop rather than a generic repair shop. It should handle both normal repair/service work and complex long-term performance builds.

## 3. Business Context

The initial business context is a Porsche/BMW performance automotive shop planned for the Sacramento, California area. The founder has direct experience working at Performance Technic in Fremont, California and has firsthand exposure to limitations in current shop management workflows.

The software should support the launch and growth of Dell'Aquila Performance Group while remaining flexible enough to become a broader software product for other specialty automotive shops in the future.

## 4. Product Goals

### 4.1 Business Goals

- Operate a new performance shop efficiently from launch.
- Reduce manual administrative work for owner/advisor staff.
- Improve communication transparency with customers.
- Increase estimate approval rate and average repair order value.
- Track vehicle history, modification history, and deferred work accurately.
- Improve technician productivity and accountability.
- Track revenue, parts margins, labor sales, and work-in-progress.
- Support growth from a small startup shop to a larger multi-technician operation.

### 4.2 Product Goals

- Provide a clean customer and vehicle database.
- Build estimates quickly using labor, parts, fees, discounts, and canned jobs.
- Convert approved estimates into repair orders and invoices.
- Track appointment, repair order, parts, approval, and payment statuses.
- Enable photo/video documentation and digital inspections.
- Support customer approvals and payments through digital links.
- Provide dashboards for owners, advisors, technicians, and parts staff.
- Support performance-build records and platform-specific service packages.

## 5. Target Users

### 5.1 Owner / Manager

The owner or manager needs full operational and financial visibility. This user manages shop workload, staff performance, revenue, profitability, customer satisfaction, and strategic planning.

Key needs:

- Owner dashboard.
- Revenue and gross profit reporting.
- Open estimate and approval tracking.
- Work-in-progress visibility.
- Technician productivity reporting.
- Parts margin visibility.
- Accounts receivable visibility.
- Customer retention and referral tracking.

### 5.2 Service Advisor

The service advisor manages intake, customer communication, estimates, approvals, scheduling, and invoicing.

Key needs:

- Fast customer and vehicle lookup.
- Estimate builder.
- Canned jobs and packages.
- Digital inspection review.
- Approval tracking.
- SMS/email communication.
- Parts and labor visibility.
- Invoice and payment workflow.

### 5.3 Technician

Technicians need a simple workflow for assigned work, vehicle information, inspections, documentation, labor tracking, and quality control.

Key needs:

- Assigned job list.
- Repair order details.
- Vehicle history and modification notes.
- Digital inspection forms.
- Photo/video uploads.
- Time tracking.
- Parts status.
- Internal notes.
- Quality control checklist.

### 5.4 Parts Manager

The parts manager sources, orders, receives, returns, and tracks parts.

Key needs:

- Parts list by repair order.
- Vendor database.
- Purchase orders.
- Receiving workflow.
- Backorder and ETA tracking.
- Inventory lookup.
- Cost, sale price, and margin visibility.

### 5.5 Customer

Customers need a premium and transparent digital experience.

Key needs:

- Appointment confirmations and reminders.
- Estimate review and approval links.
- Inspection photos/videos.
- Status updates.
- Invoice and payment links.
- Service history access in a future portal.

## 6. Core Functional Requirements

### 6.1 Customer Management

The system shall allow users to create, search, update, and archive customer profiles.

Customer profiles shall support:

- First name and last name.
- Company name.
- Phone number.
- Email address.
- Physical address.
- Preferred contact method.
- Referral source.
- Tags such as VIP, fleet, wholesale, referral, or problem customer.
- Internal notes.
- Communication history.
- Customer since date.
- Total spend.
- Open balance.
- Associated vehicles.

Users shall be able to search customers by name, phone, email, VIN, license plate, or vehicle description.

### 6.2 Vehicle Management

The system shall maintain detailed records for every vehicle.

Vehicle profiles shall support:

- VIN.
- Year, make, model, trim, and engine.
- License plate.
- Color.
- Mileage history.
- Service history.
- Modification history.
- Warranty notes.
- Track-use status.
- Vehicle photos.
- Internal vehicle notes.

Performance-shop-specific vehicle fields should include:

- Engine modifications.
- Suspension setup.
- Brake setup.
- Wheel and tire setup.
- Alignment specifications.
- Tune or software version.
- ECU/TCU tuning information.
- Dyno results.
- Fluids used.
- Known issues.
- Track event history.
- Previous shop history.

The system should support platform tags for common BMW and Porsche platforms, including BMW E36, E46, E9X, F8X, G8X and Porsche 996, 997, 991, 992, Cayman, Boxster, Macan, and Cayenne.

### 6.3 Appointment Scheduling

The system shall provide appointment scheduling for drop-offs, pickups, waiter appointments, inspections, internal work blocks, tow-ins, and track-prep deadlines.

Scheduling views should include:

- Daily calendar.
- Weekly calendar.
- Technician calendar.
- Bay/lift calendar.
- Appointment list view.

Appointment statuses should include:

- Requested.
- Confirmed.
- Dropped off.
- Awaiting inspection.
- Inspection in progress.
- Estimate pending.
- Waiting for approval.
- Approved.
- Waiting for parts.
- In progress.
- Quality control.
- Ready for pickup.
- Picked up.
- Cancelled.
- No-show.

### 6.4 Estimate Management

The system shall allow service advisors to create professional estimates from customer and vehicle profiles.

Estimate functionality shall include:

- Labor line items.
- Parts line items.
- Shop supplies.
- Sublet work.
- Taxes and fees.
- Discounts.
- Recommended services.
- Canned jobs and reusable packages.
- Customer-visible notes.
- Internal-only notes.
- Photos and videos.
- Digital approval links.
- Approval or decline by individual line item.
- Revision history.
- Conversion to repair order.
- Conversion to invoice when applicable.

Example performance-shop packages should include:

- BMW F80 crank hub service.
- BMW E46 M3 rod bearing service.
- Porsche 996 IMS service.
- Porsche 991 major service.
- Pre-purchase inspection.
- Track inspection.
- Brake fluid flush.
- Corner balance and alignment.
- Coilover installation.
- Exhaust installation.
- Turbo upgrade package.
- Cooling system refresh.

### 6.5 Repair Order Management

The system shall convert approved estimates into active repair orders.

Repair order functionality shall include:

- Advisor assignment.
- Technician assignment.
- Job status tracking.
- Parts status tracking.
- Labor time tracking.
- Technician notes.
- Internal-only comments.
- Customer-visible comments.
- Photo and video upload.
- Additional work requests.
- Customer approval for additional work.
- Job hold or pause reasons.
- Quality control checklist.
- Conversion to invoice.

Repair order statuses should include:

- Open.
- Awaiting diagnosis.
- Diagnosis in progress.
- Estimate needed.
- Waiting for customer approval.
- Waiting for parts.
- Parts arrived.
- Ready for technician.
- Work in progress.
- Waiting on sublet.
- Quality control.
- Ready for invoice.
- Ready for pickup.
- Closed.

### 6.6 Digital Vehicle Inspection

The system shall support digital vehicle inspections performed from a tablet, laptop, or workstation.

Inspection functionality shall include:

- Reusable inspection templates.
- Good, caution, and failed statuses.
- Technician notes.
- Photo uploads.
- Video uploads.
- Customer-visible findings.
- Internal-only findings.
- Recommended repair creation.
- Conversion of recommendations into estimate line items.

Suggested inspection templates include:

- General safety inspection.
- Pre-purchase inspection.
- Track readiness inspection.
- BMW performance inspection.
- Porsche performance inspection.
- Oil leak inspection.
- Suspension inspection.
- Brake inspection.
- Cooling system inspection.

### 6.7 Technician Workflow

The technician interface shall prioritize clarity and speed.

Technicians shall be able to:

- View assigned repair orders.
- View priority and promised completion date.
- View vehicle information and history.
- Clock in and out of jobs.
- Add notes.
- Upload photos and videos.
- Request parts.
- Flag blockers or concerns.
- Mark tasks complete.
- Request advisor review.
- Submit work for quality control.

The technician dashboard should show:

- Jobs assigned today.
- Jobs waiting on parts.
- Jobs ready to start.
- Blocked jobs.
- Labor hours sold.
- Labor hours completed.
- Technician efficiency metrics.
- Comeback or warranty jobs.

### 6.8 Parts Management

The system shall manage parts from estimate through installation.

Parts functionality shall include:

- Part number.
- Brand.
- Description.
- Quantity.
- Cost.
- Sale price.
- Margin.
- Vendor.
- ETA.
- Repair order assignment.
- Purchase order creation.
- Receiving.
- Returns.
- Core tracking.
- Backorder tracking.

Part statuses should include:

- Needed.
- Quoted.
- Ordered.
- Backordered.
- In transit.
- Arrived.
- Installed.
- Returned.
- Cancelled.

### 6.9 Inventory Management

The system should support inventory management for stocked parts, fluids, tires, and shop supplies.

Inventory functionality should include:

- Quantity on hand.
- Minimum stock level.
- Reorder alerts.
- Cost.
- Sale price.
- Vendor.
- Brand.
- Part number.
- Location or bin.
- Barcode or QR code support.
- Inventory adjustments.
- Stock usage on repair orders.

Common inventory categories include engine oil, brake fluid, transmission fluid, coolant, filters, brake pads, brake rotors, spark plugs, hardware, tires, track consumables, alignment parts, and detailing supplies.

### 6.10 Invoicing and Payments

The system shall create invoices from completed repair orders.

Invoice functionality shall include:

- Taxes and fees.
- Deposits.
- Discounts.
- Partial payments.
- Full payments.
- Payment links.
- Receipts.
- Refunds and voids.
- Open balance tracking.
- Accounting export or sync.

Supported payment methods should include cash, card, ACH, check, financing, and third-party payment providers.

Potential payment integrations include Stripe, Square, Authorize.net, and QuickBooks Payments.

### 6.11 Customer Communication

The system shall centralize customer communication.

Communication functionality should include:

- SMS messages.
- Email messages.
- Appointment reminders.
- Estimate approval links.
- Invoice payment links.
- Inspection result links.
- Status updates.
- Pickup notifications.
- Payment reminders.
- Follow-up messages.
- Review requests.
- Communication history on the customer record.

Suggested message templates include appointment confirmation, vehicle received, inspection completed, estimate ready, approval reminder, parts delay, work started, work completed, ready for pickup, payment reminder, thank-you message, and review request.

### 6.12 Workflow Board

The system shall provide a visual workflow board for all active vehicles.

Workflow columns should include:

- Scheduled.
- Dropped off.
- Waiting for inspection.
- Waiting for estimate.
- Waiting for approval.
- Waiting for parts.
- Ready to work.
- In progress.
- Quality control.
- Ready for pickup.

Each workflow card should show:

- Customer name.
- Vehicle.
- Repair order number.
- Advisor.
- Technician.
- Priority.
- Promise date.
- Parts status.
- Approval status.
- Balance due.

### 6.13 Performance Build Management

The system should support long-term performance builds and project vehicles.

Build management functionality should include:

- Build profile.
- Vehicle platform.
- Customer goals.
- Intended use.
- Street, track, autocross, daily driver, or race car designation.
- Power goals.
- Suspension goals.
- Brake goals.
- Budget.
- Project phases.
- Current modifications.
- Planned modifications.
- Completed modifications.
- Installed parts.
- Dyno graphs.
- Alignment sheets.
- Tune references or file references.
- Future upgrade plans.

## 7. Reporting and Analytics

The system should provide owner and management reporting.

Reports should include:

- Revenue.
- Gross profit.
- Labor sales.
- Parts sales.
- Average repair order value.
- Technician efficiency.
- Estimate approval rate.
- Declined work.
- Deferred work.
- Customer retention.
- New customers.
- Car count.
- Shop capacity.
- Open repair orders.
- Accounts receivable.
- Parts margins.
- Comebacks and warranty work.

The owner dashboard should show today’s appointments, vehicles currently in the shop, open estimates, waiting approvals, waiting parts, weekly revenue, monthly revenue, unpaid invoices, technician productivity, and average repair order value.

## 8. Roles and Permissions

The system shall support role-based permissions.

Required roles include:

- Owner/Admin.
- Manager.
- Service Advisor.
- Technician.
- Parts Manager.
- Bookkeeper.
- Customer.

Permission rules should prevent users from accessing functionality outside their job responsibilities. For example, technicians should be able to view assigned work, add notes, upload photos, complete inspections, and track time, but they should not necessarily be able to view full job profitability, delete customer records, or modify invoices.

## 9. Integrations

Recommended integrations include:

- QuickBooks Online for accounting.
- Stripe or Square for payments.
- Twilio for SMS messaging.
- SendGrid or Postmark for email.
- NHTSA VIN decoder or a commercial VIN data provider.
- Google Calendar or Outlook Calendar.

Future parts and vendor integrations may include Worldpac, SSF Auto Parts, FCP Euro, Pelican Parts, tire distributors, and other vendor APIs where available.

## 10. Non-Functional Requirements

### 10.1 Usability

The system should be fast, clean, modern, mobile-friendly, tablet-friendly, searchable, and efficient for daily use. Common workflows should require minimal clicks.

### 10.2 Performance

The system should load main pages in under two seconds under normal usage, support fast customer and vehicle search, and handle multiple users working simultaneously.

### 10.3 Security

The system shall require authentication, support role-based access control, encrypt sensitive data, avoid storing raw payment card data, and maintain audit logs for important actions.

### 10.4 Reliability

The system should be cloud-hosted, backed up regularly, resistant to accidental deletion of critical records, and reliable enough for daily shop operations.

### 10.5 Scalability

The system should scale from one shop to multiple locations, from a few employees to larger teams, and from hundreds of customers to tens of thousands of customer and vehicle records.

## 11. MVP Scope

### 11.1 MVP In Scope

The first usable version should include:

- Customer database.
- Vehicle database.
- Estimate builder.
- Repair order builder.
- Invoice builder.
- Basic scheduling.
- Basic workflow statuses.
- Technician assignment.
- Parts and labor line items.
- Customer approval by link or email.
- Basic payment recording or payment links.
- Basic reporting.
- Internal notes.
- Photo uploads.

### 11.2 MVP Out of Scope

The first version can defer:

- Full inventory management.
- Advanced QuickBooks synchronization.
- Full customer portal.
- Advanced technician efficiency analytics.
- Full parts vendor integrations.
- Loaner vehicle management.
- Full performance build management.
- Advanced marketing automation.

## 12. Roadmap

### Version 1: Core Shop Operations

Focus on customers, vehicles, estimates, repair orders, invoices, scheduling, basic approvals, and basic payment tracking.

### Version 2: Communication and Technician Workflow

Add SMS/email templates, digital inspections, technician dashboards, photos/videos, and a workflow board.

### Version 3: Parts and Inventory

Add purchase orders, parts receiving, inventory, vendor management, core tracking, returns, and margin tracking.

### Version 4: Performance Shop Features

Add build profiles, modification history, dyno/alignment tracking, track-prep templates, platform-specific job packages, and project phases.

### Version 5: Advanced Analytics and Integrations

Add QuickBooks sync, payment processing automation, advanced reports, customer portal, marketing follow-ups, and multi-location support.

## 13. Example End-to-End Workflow

1. Customer contacts the shop.
2. Advisor creates or finds the customer profile.
3. Advisor creates or finds the vehicle profile.
4. Advisor schedules the appointment.
5. Customer receives appointment confirmation.
6. Vehicle is dropped off.
7. Advisor opens a repair order.
8. Technician performs inspection or diagnosis.
9. Technician adds notes, photos, and findings.
10. Advisor builds an estimate.
11. Customer receives and approves or declines estimate items.
12. Approved work becomes active repair order work.
13. Parts are ordered or pulled from inventory.
14. Technician performs approved work.
15. Technician submits completed work for quality control.
16. Advisor converts the repair order to an invoice.
17. Customer receives invoice and payment link.
18. Customer pays and picks up the vehicle.
19. System sends follow-up or review request.

## 14. Draft Data Model

### Customer

- Customer ID.
- First name.
- Last name.
- Company name.
- Phone.
- Email.
- Address.
- Preferred contact method.
- Tags.
- Notes.
- Created date.

### Vehicle

- Vehicle ID.
- Customer ID.
- VIN.
- Year.
- Make.
- Model.
- Trim.
- Engine.
- Mileage.
- License plate.
- Color.
- Notes.

### Estimate

- Estimate ID.
- Customer ID.
- Vehicle ID.
- Status.
- Created date.
- Expiration date.
- Line items.
- Total.
- Approval status.

### Repair Order

- Repair order ID.
- Estimate ID.
- Customer ID.
- Vehicle ID.
- Advisor ID.
- Technician ID.
- Status.
- Open date.
- Promise date.
- Completed date.
- Notes.

### Invoice

- Invoice ID.
- Repair order ID.
- Customer ID.
- Vehicle ID.
- Status.
- Total.
- Balance due.
- Payment status.

### Part

- Part ID.
- Part number.
- Brand.
- Description.
- Cost.
- Sale price.
- Vendor.
- Status.

### Labor Item

- Labor ID.
- Description.
- Hours.
- Rate.
- Technician.
- Status.

## 15. Initial User Stories and Acceptance Criteria

### Story 1: Create a Customer

As a service advisor, I want to create a customer profile so that I can associate vehicles, appointments, estimates, repair orders, invoices, and communication history with that customer.

Acceptance criteria:

- User can enter customer name, phone, email, address, preferred contact method, referral source, tags, and notes.
- User can save the customer record.
- User can search for the customer after saving.
- User can associate one or more vehicles with the customer.

### Story 2: Create a Vehicle

As a service advisor, I want to create a vehicle profile so that the shop can track service history, mileage, and modification details.

Acceptance criteria:

- User can enter VIN, year, make, model, trim, engine, mileage, plate, and color.
- User can associate the vehicle with a customer.
- User can add internal notes and performance-specific details.
- User can view the vehicle from the customer profile.

### Story 3: Build an Estimate

As a service advisor, I want to create an estimate with labor and parts so that the customer can approve recommended work.

Acceptance criteria:

- User can add labor line items.
- User can add parts line items.
- User can add fees, discounts, and taxes.
- User can use canned jobs.
- User can send the estimate to the customer.
- Customer can approve or decline individual line items.

### Story 4: Convert Estimate to Repair Order

As a service advisor, I want approved estimate items to become a repair order so that technicians can perform the work.

Acceptance criteria:

- User can convert approved estimate items into a repair order.
- Declined items remain tracked as declined or deferred work.
- User can assign a technician.
- Repair order status starts as open or ready for technician.

### Story 5: Technician Completes Work

As a technician, I want to view assigned repair orders and mark tasks complete so that the advisor can track progress and invoice the customer.

Acceptance criteria:

- Technician can view assigned repair orders.
- Technician can add notes, photos, and videos.
- Technician can clock in and out of work.
- Technician can mark tasks complete.
- Technician can submit work for quality control.

### Story 6: Invoice and Payment

As a service advisor, I want to convert completed work into an invoice and send a payment link so that the customer can pay before pickup.

Acceptance criteria:

- User can convert a completed repair order into an invoice.
- Invoice includes approved labor, parts, taxes, fees, deposits, and discounts.
- User can send invoice to customer.
- Customer can access a payment link if payment integration is enabled.
- Payment status updates after payment is recorded or received.

## 16. Recommended Technology Approach

A practical modern web application stack should include:

- Frontend: React, Next.js, and Tailwind CSS.
- Backend: Node.js with NestJS, Python with Django/FastAPI, or Ruby on Rails.
- Database: PostgreSQL.
- Authentication: Auth0, Clerk, Supabase Auth, or custom role-based authentication.
- File storage: AWS S3, Cloudflare R2, or Supabase Storage.
- Payments: Stripe.
- Messaging: Twilio for SMS and SendGrid or Postmark for email.
- Hosting: Vercel, Render, Fly.io, AWS, or Google Cloud.

For a fast MVP, the recommended stack is either Next.js, PostgreSQL, Supabase, Stripe, and Twilio, or Ruby on Rails, PostgreSQL, Stripe, and Twilio.

## 17. Open Questions

- How many employees will use the system at launch?
- Will the owner be the only advisor initially?
- Will technicians need tablet access in the shop?
- Should customers approve estimates by text message from day one?
- Is built-in payment processing required on day one?
- Is QuickBooks integration required on day one?
- Is the software only for Dell'Aquila Performance Group, or should it eventually be sold to other shops?
- Should inventory be included in the MVP?
- Are parts vendor integrations needed in the MVP?
- Should a customer portal be included in the MVP or deferred?
- Should technician efficiency be tracked from day one?
- Which Porsche/BMW canned jobs should be built first?
- Should the first interface be desktop-first, tablet-first, or mobile-first?

## 18. Recommendation

The recommended plan is to prioritize a business-ready MVP for operating Dell'Aquila Performance Group at launch. The MVP should focus on customers, vehicles, estimates, repair orders, invoices, basic scheduling, technician assignment, line items, digital approvals, payment recording, notes, and photo uploads.

After the shop workflow is validated, the product can expand into communication automation, digital inspections, parts and inventory, performance build management, advanced reporting, accounting integrations, payment automation, and customer portal features.
