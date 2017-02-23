# hackaton-texting

<strong>Project Idea:</strong> Enable subscription management via (SMS) text message. OrderGroove would power text message notifications that would enable a customer to make a change to a subscription or order.

<strong>Project’s Why?</strong>
<ul>
  <li>OrderGroove’s Mission statement is “Transforming commerce, one relationship at a time to create a world where you have more time for the moments that matter in life”</li>
  <li>Provide the subscriber with greater control over subscriptions and their orders</li>
  <li>Create a more frictionless experience than visiting the MSI to manage subscriptions</li>
  <li>Improve client’s relationship with customer by reducing friction/frustration with subscription management</li>
 </ul>

<strong>SMS Subscription Management Use Cases:</strong>
<br>Current MSI functionality as a response to order reminder text:
<ol>
  <li>Send Now</li>
  <li>Skip Order</li>
  <li>Change Date</li>
  <li>Change Frequency</li>
  <li>Change quantity</li>
  <li>SKU Swap</li>
  <li>Cancel subscription</li>
  <li>Reactivate subscription</li>
 </ol>

<strong>Technical Execution:</strong>
<ol>
<li>Create mobile phone number 2-step authentication in the MSI (initial POC) and in the subscription signup flow on the order review page (to come later)
<ol>
<li>Customer enters phone number.</li>
<li>OG generates a code and sends to the phone number.</li>
<li>OG displays a message to the customer letting them know we have sent a code.</li>
<li>OG displays a place for the customer to enter the code on the frontend.</li>
<li>Customer receives a text with the code and enters it on the frontend.</li>
<li>Phone is then validated and stored in OG’s database for future communication.</li>
</ol>
</li>
<li>Hook into OG Conversations platform + Twilio middleware to trigger text communications to customers and then exchange a series of texts with the customer.</li>
</ol>
