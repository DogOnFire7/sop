# Aerodrome Flight Information Service (AFIS)

An **Aerodrome Flight Information Service** is provided at aerodromes that do not have a full air traffic control (ATC) service. The person providing it — the **Aerodrome Flight Information Service Officer (AFISO)** — gives pilots the information they need to operate safely, but does **not** control traffic, issue clearances to airborne aircraft, or provide separation. On the network, staffing an *Information* position means you are acting as an AFISO.

!!! abstract "The four golden rules"
    1. **You provide information — you do not control.** No clearances to aircraft in the air, no mandatory instructions, no sequencing.
    2. **Pilots separate themselves.** You never provide separation. You give traffic information; the pilot builds their own picture and stays clear.
    3. **Phraseology reflects this.** Use *"at your discretion"*, *"report…"*, and *"traffic is…"*. Never say *"cleared"*.
    4. **When in doubt, pass information and let the pilot decide.**

---

## 1. Scope of the Service

!!! info "What AFIS *is*"
    - An **information** service and an **alerting** service for a defined aerodrome and its immediate vicinity (typically the aerodrome traffic zone / circuit).
    - A source of **traffic information**, **meteorological information**, and **aerodrome information** to help pilots make their own decisions.
    - A relay point for **ATC clearances** issued by a controlling unit (Approach / Area), where one is online.

!!! danger "What AFIS is **not**"
    - AFIS is **not** air traffic control. You have **no authority** to instruct an airborne aircraft.
    - You do **not** provide separation between aircraft, or between aircraft and obstacles. The pilot is always responsible for their own separation and collision avoidance.
    - You do **not** issue take-off, landing, or airways clearances on your own authority.

---

## 2. AFIS vs Aerodrome Control (Tower)

The single most important thing to understand is how an Information position differs from a Tower. If you are used to controlling, the change in mindset is the hard part — not the phraseology.

| Aspect | Aerodrome Control (**Tower**) | Aerodrome Flight Information Service (**Information**) |
|---|---|---|
| Spoken callsign | "… Tower" | "… Information" |
| Authority | Issues clearances and instructions; traffic complies | Provides information only; no clearances to airborne aircraft |
| Separation | Provided by the controller | The pilot's responsibility |
| Take-off / landing | "Cleared for take-off" / "Cleared to land" | "Take off at your discretion" / "Land at your discretion" |
| Runway in use | Assigned by the controller | Advised only; a pilot may request another and use it at their discretion |
| Sequencing | Controller sequences arrivals and departures | Pilots self-sequence using the traffic information passed |
| Airspace | Controlled (typically Class D around the field) | Uncontrolled airspace / aerodrome traffic zone |

---

## 3. Callsign and Position Conventions

The **radiotelephony callsign** always ends in **Information** — this is how pilots know they are talking to an information service and not a control position.

| Location | Spoken callsign |
|---|---|
| Gan International | Gan Information |
| Hanimaadhoo | Hanimaadhoo Information |
| A Sri Lankan domestic field | *(Location)* Information |

!!! note "Network login callsign"
    Your **login callsign** on the network (e.g. the suffix used when you connect) is set by the SRM vACC controller pack / roster configuration, and any rating or endorsement requirements to staff the position are defined by the vACC. This document covers **how to operate** the service, not who is permitted to log on — check your vACC's controlling policy for that.

---

## 4. Responsibilities

Keeping these two columns straight in your head is the whole job.

| The **AFISO** provides | The **pilot** is responsible for |
|---|---|
| Traffic information on known aircraft | Separation from all other traffic |
| Meteorological information (QNH, wind, etc.) | Deciding when to taxi, take off and land |
| Aerodrome information (runway in use, surface state, hazards) | Collision avoidance |
| Relaying ATC clearances from the controlling unit | Compliance with the rules of the air |
| Initiating alerting action for aircraft in difficulty | The ultimate safe conduct of the flight |

!!! warning "Regulatory note — ground movements"
    Some real-world authorities allow an AFISO to pass *instructions* to traffic on the manoeuvring area (taxiways and runways) while still providing information-only to aircraft in flight. The **airborne information-only principle is universal**. For consistency on the network, treat **all** AFIS transmissions as information and use *"at your discretion"* phraseology unless your vACC specifies otherwise.

---

## 5. The Services in Detail

### 5.1 Traffic information

Pass timely, relevant information about any traffic you are aware of so pilots can self-separate. Keep it factual and concise:

> **type / callsign — position or direction — level (if known) — intentions**

!!! example "Traffic information format"
    - "Traffic is a DHC-6 Twin Otter, joining left base runway 10, ahead of you."
    - "Traffic is a Cessna, 5 miles to the north, 2,000 feet, inbound."
    - "No reported traffic."

Use *"no reported traffic"* rather than *"the runway is clear"* unless you can positively see it is — you are reporting what you *know*, not guaranteeing what is *true*.

### 5.2 Meteorological information

Provide, as available: **surface wind**, **QNH**, visibility, cloud, temperature and dewpoint, and any significant weather. QNH and wind are the essential items on first contact and before departure/arrival.

### 5.3 Aerodrome information

Anything affecting the safe use of the aerodrome: the **runway in use**, surface state (wet, water, contamination), work in progress, unserviceable equipment or lighting, obstructions, bird activity, and — very relevant in the region — **water on the runway** and nearby **seaplane / water-aerodrome activity**.

### 5.4 Runway in use

You **advise** a runway in use, normally the one best aligned with the surface wind. It is advisory: a pilot may elect to use another runway and does so at their own discretion, self-separating from other traffic. Never present the runway as an instruction.

### 5.5 Relaying ATC clearances

You do not issue airways/IFR clearances on your own authority. Where an Approach or Area controller is online, IFR clearances are **obtained from and relayed via** that unit, and any assigned squawk comes from them. Where no controlling unit is online, standard network procedures apply and IFR aircraft depart at their discretion, obtaining onward clearance from the next unit or self-briefing as appropriate.

---

## 6. Phraseology

### 6.1 Say / don't say

!!! failure "Do **not** say (these are control instructions)"
    - "Cleared for take-off" / "Cleared to land"
    - "Line up and wait"
    - "You are number two, follow the…"
    - "Cleared to taxi to holding point…"

!!! success "Say instead (information)"
    - "Take off at your discretion" / "Land at your discretion"
    - "Report ready for departure" / "Report final" / "Report airborne"
    - "Traffic is… , report when you have it in sight" *(pilots self-sequence)*
    - "Runway 10 in use, taxi via Alpha at your discretion"

### 6.2 By phase of flight

Worked examples below use a generic callsign, `8Q-XYZ`. Flight-number callsigns (e.g. an airline flight) are handled identically. Wind is written in full as it would be spoken.

!!! example "Start-up & push-back"
    ```text
    PILOT:  Gan Information, 8Q-XYZ, stand 3, request start-up, IFR to Male.
    AFIS:   8Q-XYZ, Gan Information, runway 10 in use, wind 090 degrees 8 knots,
            QNH 1011, start up at your discretion, report ready to taxi.
    ```

!!! example "Taxi"
    ```text
    PILOT:  Gan Information, 8Q-XYZ, request taxi.
    AFIS:   8Q-XYZ, runway 10, taxi via Alpha at your discretion, QNH 1011,
            traffic is one Twin Otter vacated at the north apron.
    ```

!!! example "Departure"
    ```text
    PILOT:  Gan Information, 8Q-XYZ, ready for departure runway 10.
    AFIS:   8Q-XYZ, runway 10, wind 090 degrees 8 knots, no reported traffic,
            take off at your discretion, report airborne.
    PILOT:  Airborne, 8Q-XYZ.
    AFIS:   8Q-XYZ, roger, when ready contact Male Approach 119.100.
    ```

!!! example "Traffic circuit / pattern"
    ```text
    PILOT:  8Q-XYZ, downwind runway 10, touch and go.
    AFIS:   8Q-XYZ, roger, traffic is a Cessna on a 4 mile final runway 10,
            report final number two.
    ```
    *You pass the traffic so the pilot can slot in behind it — you do not order the sequence.*

!!! example "Arrival & landing"
    ```text
    PILOT:  Gan Information, 8Q-XYZ, 15 miles north, 3,000 feet, inbound, request joining information.
    AFIS:   8Q-XYZ, Gan Information, runway 10, QNH 1011, wind 090 degrees 8 knots,
            one aircraft in the left-hand circuit, report joining.
    PILOT:  8Q-XYZ, final runway 10.
    AFIS:   8Q-XYZ, runway 10, wind 090 degrees 8 knots, preceding traffic
            a Twin Otter vacating, land at your discretion.
    ```

---

## 7. IFR Operations and Coordination

- **With Approach / Area:** coordinate IFR arrivals and departures with the controlling unit — relay clearances, agree release of departures, and hand traffic off at the appropriate point. The AFIS does not release or sequence IFR traffic on its own authority; that rests with the controlling unit.
- **Vertical/lateral limits:** the information service covers the aerodrome and its immediate vicinity (the traffic zone / circuit). Beyond that, aircraft are with the relevant Approach, Area, or flight information unit.
- **Transponder / squawk:** relay codes assigned by the controlling unit; where none is online, standard network conventions apply.

---

## 8. Top-Down Coverage on the Network

- If **no Information position is online**, the aerodrome is covered **top-down** by the next-higher position online (Approach, then Area), following the network's top-down principle.
- If you **are online** as Information, you are the aerodrome-level service; Approach and Area handle everything above and around you.
- You may frequently be the **only unit online** for the field. That is normal for an information position — pilots still self-separate; you simply provide the best picture you can.

---

## 9. Emergencies and Alerting

Providing the **alerting service** is a core AFISO duty. If an aircraft is in difficulty, is overdue, or declares an emergency:

1. Acknowledge, and offer assistance and information (weather, runway, known traffic, distances).
2. Do **not** attempt to "control" the aircraft — continue to provide information and let the pilot fly the aircraft.
3. **Initiate alerting action:** notify the appropriate controlling unit / supervisor so that emergency and rescue services can be alerted.
4. Keep other traffic informed so they can stay clear of the aircraft in difficulty.

---

## 10. Local Considerations — Maldives & Sri Lanka

!!! tip "Region-specific notes"
    - **ICAO phraseology** is the standard throughout the region — the conventions in this document apply directly.
    - **Water and seaplane operations** are common in the Maldives. Pass information on seaplane / water-aerodrome activity and floating traffic where relevant, and remember that surface state on water and amphibious operations affect nearby traffic.
    - **Wet runways** and heavy rain are frequent — surface state is an essential item of aerodrome information.
    - Many candidate AFIS fields are **domestic / regional airports** served by turboprop and GA traffic rather than heavy jets; tailor your traffic information accordingly.

---

## Quick Reference

| Situation | AFIS response |
|---|---|
| First contact | Callsign, runway in use, wind, QNH |
| Requesting start / taxi | Runway, QNH, traffic, "at your discretion" |
| Ready for departure | Runway, wind, traffic, "take off at your discretion, report airborne" |
| In the circuit | Pass traffic, "report final" — pilots self-sequence |
| On final | Runway, wind, traffic, "land at your discretion" |
| Aircraft in difficulty | Provide information, **initiate alerting action**, keep other traffic clear |
| No Information online | Covered top-down by Approach / Area |

---

!!! note "Rendering requirements"
    This page uses standard MkDocs Material features: **admonitions** (`admonition`), **fenced code blocks** (`pymdownx.superfences`) for the phraseology exchanges, and tables. These are enabled in a typical Material `mkdocs.yml`; if the phraseology blocks or callouts don't render, confirm `admonition` and `pymdownx.superfences` are listed under `markdown_extensions`.
