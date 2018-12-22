*Agile Ops - the process:*

**HIGH LEVEL:**

1.  We're all engineers -- begin culture shift toward a united engineering front, focus on infrastructure engineering, big teams are ok!  
1.  Buffer interrupts!  Establish Persons of the Week, on-call rotation, direct monitoring and emails only to those who should do something about it, protect the team
1.  Create a sustainable model for planned work (IDD -  Infrastructure Driven Development), begin establishing engineering credibility with the business and customers
1.  Build backlogs of planned work - business owners/dev customers/internal
1.  Get a handle on the infrastructure from the Plan/Build/Run perspective
1.  Manage, staff and grow as required

**SPECIFICS:**

1.  align dev and ops resources either as a team or teams that participate on IDD projects, no organizational silos, establish engineering as the primary competency -- differentiate as an organization operations as an umbrella, but positions within it being engineering, support, administration, testing, etc.
1.  create appropriate backlogs for:  business projects (business planned work), interrupt tasks (PoTW), automation and self-service (for dev team customers)
1.  make sure the PoTW triages absolutely everything (or perhaps the people manager or someone else as a buffer while getting this rolling) -- this will require a cultural change since everyone wants to jump in during a crisis.  Also, if there is not a solid, lightweight incident management plan in place, this is the time to do it, and set expectations so it doesn't derail the whole team.
1.  begin creating customer relationships with dev teams, discuss level of ownership and autonomy the group needs, SLA, escalation, and a plan to create sustainable patterns around the tech (ops can't do it all, so how is it going to get done?  is the team on call?  are common tasks automated or scripted? etc.)
1.  Get an ops-oriented PO who is managing the various backlogs and acting as a liaison to the business and other POs
1.  Get good at organization and make planning meetings very focused, standups based around the kanban boards for the initiatives
1.  make sure system stability and architecture (SS&A) work is prioritized because it is a huge part of building trust and morale in ops, always allocate at least a pair to this at all times
1.  build out the backlogs further and start seeing what velocity and % of interrupts are happening, and adjust staff as needed
1.  begin integrating external devs into feature development, and begin the process of distributing information
1.  maturity assessment of all technologies
1.  Work toward 100% config management as part of SS&A, never build systems manually unless you absolutely have to
1.  Work on increasing maturity of all core technologies -- many of these will be things that no one except ops "owns" so it is critical to distribute the support model along plan/build/run lines:  architecture owns the upgrades & roadmap/replacement, engineering owns how to interface with it properly, operations owns how to maintain it/recover/replace/build it 
1.  From the people perspective, begin looking at career paths from front line support all the way to Infrastructure Manager/Architect, begin pushing tools, capabilities and knowledge lower and lower in the organization, many time support/IT are a huge untapped pool of talent just looking for a way to get more experience, make this happen!
1.  If architecture is present in the org, infrastructure architect needs to be in the mix
1.  Bring operations practices and expertise into engineering (and arch), and bring engineering best practices into ops.
1.  Encourage everyone in ops to learn an object-oriented language such as Ruby, Go, Python, PHP or Java.
1.  Ensure that a culture of mastery develops and that even juniors can be feature leads

**IDD/FDD HIGH LEVEL:**

1. Just Enough Design Initially (JEDI) -- architectural planning and spikes necessary to complete the iteration (not feature) with minimal rework

2. Tackle the easy problems first

3. Assign a feature lead who will assemble the pairs necessary per iteration to estimate and complete the stories (may include customer developers!)

4. Runs like Scrum-Ban for the 2 week iterations

5. Prizes Agile principles like small batches, frequent delivery and active participation of customers in the process, PO manages this relationship

6. Teams are cross-functional and purpose-driven

7. Teams can become customers as well, meaning a IDD/FDD team may need an infrastructure feature in order to deliver, and this may constitute another team.  We don't care who the customer is, necessarily, only that we treat them all the same and with the same level of care

**INFRASTRUCTURE MATURITY:**

deep analysis...


<table>
  <tr>
   <td><strong>VECTOR</strong>
   </td>
   <td><strong>DESCRIPTION</strong>
   </td>
  </tr>
  <tr>
   <td>Supportability
   </td>
   <td>The support model in place around the infrastructure, including escalations, off-hours support and level of continual operations support, this also includes instrumentation and monitoring
   </td>
  </tr>
  <tr>
   <td>Operability
   </td>
   <td>A highly-operable infrastructure means that supporting it during normal operations (managing services, for example) is extremely straightforward.  Troubleshooting is easy, configurations are completely managed, and operational tasks can be handled by almost anyone with the requisite permissions.
   </td>
  </tr>
  <tr>
   <td>Recoverability
   </td>
   <td>The ease of which you can recover from a failure or complete loss of the infrastructure.  A high level of recoverability means it's zero downtime and auto-healing.
   </td>
  </tr>
  <tr>
   <td>Documentation
   </td>
   <td>This doesn't necessarily mean documents in the traditional sense.  It could be comments in code, readme files in github, spreadsheets, whatever.  A high level of documentation means it's easy to parse, relevant and maintained
   </td>
  </tr>
  <tr>
   <td>Architectural design maturity
   </td>
   <td>Architectural maturity means the underlying components and design are cohesive and maintained by either architecture or people acting as architects.  Good architecture encompasses related systems and means that downstream/upstream providers are also stable and mature.
   </td>
  </tr>
  <tr>
   <td>Currency
   </td>
   <td>This represents how up-to-date the system is from a patch, security, and revision level.  In the case of home-grown software, it would have an active defect management process.
   </td>
  </tr>
  <tr>
   <td>Usability
   </td>
   <td>From the developer and implementer perspective, usability means you can interface with it easily and reliably.  It doesn't have to be rocket science, and results of use are generally well-understood.  Databases like Postgres usually have high usability.
   </td>
  </tr>
  <tr>
   <td>Automation and Self-service
   </td>
   <td>This represents the programmatic solution to operations work.  This is typically the domain thought of as DevOps where deployments, provisioning, and new service generation are all done programmatically.  Developer teams, and others can do things like restart services or upgrade their own stacks without any intervention.
   </td>
  </tr>
  <tr>
   <td>Deployability
   </td>
   <td>The speed and ease which the infrastructure can be deployed from the development environment to production including all requisite testing (security, regression, compatibility, performance, etc.)
   </td>
  </tr>
  <tr>
   <td>Stability
   </td>
   <td>How often does the infrastructure fail?  High stability means almost never, and ideally without causing customer-facing service interruptions.
   </td>
  </tr>
  <tr>
   <td>Community support/adoption
   </td>
   <td>How much support and adoption is there in the world outside of the company for this infrastructure?  If it is open source, is the community actively developing and patching it?  If it's a paid product, does the vendor have a wide customer base?  Are they still going to be in business in 2 years?
   </td>
  </tr>
  <tr>
   <td>Maturity
   </td>
   <td>How long has this infrastructure been around?  If it is in-house developed, has it been in place for days?  months?  years? 
   </td>
  </tr>
  <tr>
   <td>Ease of use (inverse of complexity)
   </td>
   <td>How hard is it to work with and understand?  Nagios is an example of a highly-complex solution, where redis has high ease of use.
   </td>
  </tr>
  <tr>
   <td>Ubiquity
   </td>
   <td>How many installations or different uses are there of this technology in the infrastructure?   MongoDB is an example of an infrastructure component with high ubiquity.
   </td>
  </tr>
  <tr>
   <td>Happiness
   </td>
   <td>This is the human factor of the infrastructure.  Do people like it?  Do they enjoy working with it?   Docker is typically a high-happiness piece of infrastructure.
   </td>
  </tr>
</table>


aggregate analysis...


<table>
  <tr>
   <td>0
   </td>
   <td>No one knows anything about it, except maybe one person who no-longer works at the company.  Maybe this is technology that is no longer supported or was purchased and mothballed.  This could be internally-developed and poorly-designed or not maintained.  This is the classic thing no one will touch with a 10-foot pole.  Or, it is something completely brand-new to the company and is being championed by an individual or occasionally a team.  There's little or no recovery, fault tolerance, backups, security or documentation.  In the case of new technologies, these are probably not in production yet. 
   </td>
  </tr>
  <tr>
   <td>1
   </td>
   <td>This is something that has gotten past the initial research phase and there's some intent that it could go into production.  If it's already in production, chances are one or two people know something about it, and are constantly getting derailed from their normal work to deal with it, especially when things go wrong, or someone needs to use it.  Recoverability is largely manual and sketchy.  Security is low and probably not compliant.  Patch levels may be out of date, and people may be afraid to do too much with it because it is finicky and/or unstable.  Many people have been "burned" by this.  Maybe a replacement is on the way, maybe not.  There is some documentation but not much.  It's mostly tribal knowledge or what you can dig up on forums or vendor sites.  Chances are there is no SLA, or if there is, it gets violated.
   </td>
  </tr>
  <tr>
   <td>2
   </td>
   <td>This is something a few people are experts in and has the feel of general adoption.  There's some documentation/recovery capability, but most of what happens with it is done manually.  There is little or no self-service capability and minimal automation.  Some parts of this may be under configuration management control, but it may not be 100% up-to-date.  It may have dependencies on other barely-supported technologies and is frequently error-prone.  This may be a frequent headache for on-call support, and may trigger customer-facing outages.  It may be more current with patch levels, but there's not a real process around that.  Security holes exist in it, and most people know it.  It may have more than one installation in the company, but they would likely be inconsistently done.
   </td>
  </tr>
  <tr>
   <td>3
   </td>
   <td>Most production technologies fall into this rating.  This is something that can largely be recovered and has reasonable fault tolerance.  A lot of it is manual work, but there are at least scripts and a good amount of it under configuration management control.  Patch levels may be only a few releases behind, and there are people who do so with some regularity.  SLAs exist for this and are usually met.  People are not eager to use this infrastructure, but do so because it is considered part of the core stack.  Troubleshooting and supporting it is usually okay, but can occasionally be extremely challenging due to unusual use cases or user error.  It is not super straightforward to upgrade or manage, so these activities are usually risky and prone to rework.
   </td>
  </tr>
  <tr>
   <td>4
   </td>
   <td>This infrastructure has been around for a while.  People know how to use it, and frequently do.  It's extremely stable and reliable and kept as current as is reasonable without triggering outages.  When it fails, 90% of the time or more it is either fault-tolerant or not customer-facing.  This infrastructure requires very little after-hours support, is integrated into build pipelines and probably has extremely high test coverage.  There are plenty of people throughout the organization who are experts on it.  It's considered a core piece of technology and is prized for its ease of use, ubiquity and lack of operational/interfacing complexity.  Community support is wide, and it is relatively easy to hire people who know how to work with it and support it.  It may have a group of people who are dedicated to it in operations, and possibly engineering.  It's on the architectural roadmap.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>This is something most people know how to use, upgrade, support and recover.  90%+ of all use cases are automated or have easy-to-use self-service tooling.  It is able to be spun-up and destroyed on demand for testing and validation purposes.  It has most likely been around for a year or more in the infrastructure.  There may be specific infrastructure engineers (e.g. DBAs) associated with it.  It is secure, compliant, and scalable.  It is a low-incident generator.  It operates so smoothly that people don't have to think about it.  
   </td>
  </tr>
</table>


**AGILE ARCHITECTURE:**

1.  Focused on establishing patterns that increase engineering and operational agility
1.  Provides a lowest-cost way of exploring new technologies through prototyping and research
1.  Decentralized in practice
1.  Center of mastery and mentoring for the organization
1.  Ties organizational strategy to feasible solutions that meet business needs
1.  Guild-building so architecture is egalitarian
1.  Standards are only set where absolutely necessary -- patterns over proscription 
