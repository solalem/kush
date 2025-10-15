---
title: Home
client_logos:
  - name: "ETech"
    logo: "/kush/images/logos/customer-1.png"
  - name: "Bluespark"
    logo: "/kush/images/logos/customer-2.png"
  - name: "Perago"
    logo: "/kush/images/logos/customer-3.png"
  - name: "Tekron"
    logo: "/kush/images/logos/customer-4.png"
---

{{< hero 
    headline="Create Meaningful Impact"
    sub_headline="Modernize Your Business Processes for Maximum Efficiency. Embrace the Joy of Technological Convinience in Your Life."
    primary_button_text="Contact Us"
    primary_button_url="/kush/contact-us"
    secondary_button_text=""
    secondary_button_url="#"
    hero_image="/kush/images/hero-dashboard.svg"
    gradient-from="#dbeafe"
    gradient-to="#f3e8ff"
    gradient-angle="180"
>}}

{{< client-logos animate="false" >}}

{{< features-section 
    title="Modernizing Your IT Teams"
    description="Let us help your IT teams embrace modern Software and Hardware development processes."
>}}

{{< feature
    title="SW Development Practices and Processes"
    description="Starting form problem identification, to solution development al the way through great operational excellence, your teams need to have best practices and optimized processes"
    badge="Design"
    badgeColor="#7c3aed"
    image="/kush/images/feature-2.svg"
    buttonText="Learn More"
    buttonLink="/services/development"
    features="Continuous Delivery,Agile Methodologies,DevOps Practices,Mobing/ Pair Programming,TDD,Monitoring Tools"
    imagePosition="left"
>}}

{{< feature
    title="Legacy System Migration"
    description="Legacy systems are the back-bone of your business. But, without proper modernization process in place, they create big liablities require huge maintenance cost. Let us help you give some love to your business critical systems."
    badge="Modenization"
    badgeColor="#2563eb"
    image="/kush/images/feature-1.svg"
    buttonText="Learn More"
    buttonLink="/services/consultation"
    features="Cloud Migration,Technical Documentation,Domain Modeling,Stangler-Fig Implementation,Data Migrations,Performance Tuning"
    imagePosition="right"
>}}

{{< feature
    title="System Architecture and Design"
    description="Most business critical system can benefit from system level design work to support security, reliablity and scalablity needs. We have experience in architecting and designing systems at scale. Let us know your needs. We have few tried and tested solutions for you development and operations teams."
    badge="Development"
    badgeColor="#16a34a"
    image="/kush/images/feature-3.svg"
    buttonText="Learn More"
    buttonLink="/services/consultation/"
    features="Cloud Native Design,Solutions Architecture,Domain-Driven Design,Test-Driven Development"
    imagePosition="right"
>}}

{{< /features-section >}}


{{< section-container class="py-20 bg-gray-50" >}}
    <div class="max-w-6xl mx-auto">
        <h2 class="text-3xl font-bold text-center mb-12">And More...</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            {{< value-card 
                title="Application Software Development"
                icon="lightbulb"
                description="We work on both open source and closed source projects for different clients. Let us know your software needs. Anything from simple mobile apps, to desktop, to complex web applications."
            >}}
            {{< value-card 
                title="Aerospace Command and Control"
                icon="plane"
                description="Specializing in UAVs/drone control software technologies, we have experience in developing and integrating with proprietary and open source tools."
            >}}
            {{< value-card 
                title="GNC Research"
                icon="computer"
                description="We have experience in GNC system development for small UAVs. We can help in research, development and consultation."
            >}}
        </div>
    </div>
{{< /section-container >}}
