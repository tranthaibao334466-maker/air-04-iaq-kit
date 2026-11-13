# Project Idea — STEM Learning Kit for Indoor Air Quality

> Purpose of this file: a one-page north star. Read it before any task and check that the work still serves the idea below.
> Source brief: `requirements.docx` (topic AIR-04 – Bedroom Air Quality Monitoring).

## 1. The idea

A **learning kit in the form of an air quality meter** for **lower and upper secondary school students (THCS and THPT)**. The kit supports a **range of hands-on activities** for STEM learning in three areas:

- **IoT**: sensing, displaying, alerting, automating
- **Field surveys**: measuring and comparing real indoor and outdoor spaces
- **Scientific research**: forming a hypothesis, collecting data, analysing it, reporting

Students should work with the kit through **high-abstraction, beginner-friendly tools**, with no low-level electronics or code required to get started.

> ⚠️ **Tool names are reference examples only, not decisions.** Scratch-style block coding and Arduino are mentioned only to show the *level of abstraction* intended. The platform, programming environment, hardware and sensors are **not chosen yet**. They must come out of the Design Thinking process. The reference hardware listed in `requirements.docx` is also only a reference.

## 2. The core research project: bedroom air quality

**Monitoring bedroom air quality is the flagship research project of the kit, not just one activity among many.** The kit is designed around it, and the other activities build the skills that lead up to it.

Students run a multi-night study in a real bedroom. They:
- monitor key indoor air indicators overnight (for example CO₂, fine particles, temperature, humidity)
- mark events and phases during the night, such as opening or closing a door or window and running an air purifier
- compare ventilation and purifier scenarios
- produce a summary report from **de-identified** data

The study fits a **Citizen Science** setting: students act as researchers, and the school organises the activity.

## 3. Who it is for

- **Primary users**: THCS and THPT students, from beginners to STEM club members and science-fair (KHKT) teams.
- **Key stakeholders**: teachers who run the activities, schools that adopt the kit, and parents, whose bedrooms and consent are involved.

## 4. What the kit must be

- **Educational first.** Air quality is the real-world context that makes learning meaningful. Learning is the goal.
- **Accurate enough for real research.** Data must be trustworthy for student science projects.
- **Easy to use and compact.** Students get results quickly, inside a normal class period.
- **Flexible and customisable.** It should grow from simple measuring to student-built programs and experiments.

## 5. Key constraints

- **No medical diagnosis.** Readings and reports must never be presented as health or medical conclusions.
- **Privacy by design.** Bedroom data is highly personal. Data must be de-identified (for example by using relative timestamps) before it is shared. Minors need parental consent.
- **Must not disturb sleep.** The kit must be quiet at night and must not cause light glare in the bedroom.
- **Long, reliable overnight logging.** The kit must collect data continuously through full nights, over several consecutive nights.
- **Safe and affordable for schools.** It must be safe for students to handle, and priced for school budgets.

## 6. Alignment check (ask before each task)

1. Does this help **students learn** through IoT, surveys or research?
2. Does it serve, or lead toward, the **bedroom air quality research project**?
3. Does it respect the **constraints**: no diagnosis, privacy, quiet at night, reliable logging, safe and affordable?
4. Am I treating a specific tool or hardware choice as a **decision** when it is still only a reference?
