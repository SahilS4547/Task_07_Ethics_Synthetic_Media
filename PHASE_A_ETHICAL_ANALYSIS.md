# Phase A: Ethical Analysis of Synthetic Representation

## Introduction

Research Task 6 gave me direct experience creating and evaluating
synthetic media rather than only reading about it. I created two final
synthetic artifacts: a talking-avatar video using D-ID Video Studio and
an audio narration using ElevenLabs. I also experimented with DeeVid AI,
although that attempt produced a sports montage rather than the
talking-presenter format I needed.

For the D-ID artifact, I used a generic stock avatar and a synthetic
voice. For the ElevenLabs artifact, I used the stock conversational
voice "Zan." I intentionally avoided cloning the voice or likeness of
a real identifiable person.

The content itself was also not fabricated. The artifacts communicated
the analytical sports narrative developed in the earlier research task.

At the time, these choices made the project relatively low risk.
However, completing the project made me realize that the same technical
capability can become ethically very different when truthfulness,
consent, context, or scale changes.

The important question is therefore not simply whether synthetic media
is good or bad. The more useful question is what conditions make a
particular use acceptable, risky, deceptive, or unacceptable.


## 1. Returning to What I Built

Revisiting my Task 6 artifacts after completing the production process
changed how I viewed them.

The D-ID video was approximately one and a half minutes long and
presented the complete coach-advisory narrative through a synthetic
talking avatar. The presenter looked professional, the background was
stable, and the mouth generally followed the narration.

However, close inspection revealed limitations. Facial expressions
were restricted, head and mouth movements became repetitive, and
emotional emphasis did not always match the meaning of the script.
Longer sentences occasionally produced less natural synchronization.

The ElevenLabs audio created a different experience. The voice was
clear, professionally paced, and free from background noise. During a
short listen, it could plausibly be interpreted as an ordinary
professional voice-over.

Over a longer listen, however, the synthetic characteristics became
more noticeable. The pacing was consistently controlled, emotional
variation was limited, and natural breathing and hesitation were
reduced.

One of the most important observations from Task 6 was that neither
artifact needed to be perfect to be convincing.

A viewer does not always carefully inspect an entire video. Someone
scrolling through content on a phone may only watch a few seconds.
Likewise, someone hearing a short audio clip may not listen long enough
to notice the unusually consistent rhythm.

This changed how I thought about synthetic-media risk. The important
threshold is not necessarily whether an artifact can survive forensic
inspection. A synthetic artifact may influence someone long before
careful inspection occurs.

I also learned how accessible production has become. I did not need to
train a machine-learning model, own specialized hardware, or understand
advanced computer graphics. Consumer-facing interfaces performed most
of the technical generation.

That accessibility is useful for legitimate applications, but it also
reduces the technical barrier for misuse.


## 2. Ethical Reasoning Across Four Axes

### 2.1 Truth Axis

My Task 6 artifacts communicated information that I had already
developed and verified. Synthetic media changed the method of delivery,
not the underlying claims.

The ethical situation changes substantially when the same delivery
mechanism communicates false information.

Consider a hypothetical example involving a large company's CEO.
Someone creates a synthetic video in which the CEO appears to announce
that the company has unexpectedly lost its largest customer and expects
a major decline in revenue.

The statement is completely fabricated.

The synthetic video is posted online shortly before financial markets
open. Employees share it internally, investors react to it, and
journalists begin trying to confirm the announcement.

Eventually the company explains that the video is fake.

The correction does not eliminate everything that happened before the
verification.

This scenario demonstrates something I did not fully appreciate before
Task 6. Synthetic media can give fabricated information the visual and
vocal characteristics that people normally associate with direct human
testimony.

The ethical problem is therefore larger than simply "AI created false
information." The synthetic representation can borrow credibility from
the appearance of a recognizable human speaker.

My Task 6 artifact was relatively safe because the underlying narrative
was truthful and the presenter was generic. Removing truthfulness while
keeping the same delivery capability changes the ethical character of
the artifact.


### 2.2 Consent Axis

Consent creates another independent boundary.

Imagine that a university communications employee wants to create a
video featuring the university president.

Instead of scheduling a recording, the employee collects publicly
available speeches and photographs and creates a synthetic version of
the president. The script contains completely accurate information
about a university program.

The information is true.

However, the president never agreed to appear in the synthetic video.

This scenario demonstrates why truthfulness alone is insufficient.

The resulting video communicates something the president may agree
with factually while simultaneously creating the false impression that
the president personally delivered or approved that particular
communication.

The problem is the appropriation of identity.

My Task 6 project avoided this problem by using a generic stock avatar
and stock synthetic voices. I deliberately did not clone a real
person's voice.

That decision now appears more significant than it did while I was
simply trying to satisfy the technical requirements of Task 6.

Using someone's public photograph, speech, or recording does not
automatically mean that person has consented to having an artificial
version of themselves created.

For responsible synthetic media, consent therefore needs to concern
not only access to source material but authorization for the specific
synthetic representation and its intended use.


### 2.3 Context Axis

My Task 6 repository clearly identifies the artifacts as synthetic.

The D-ID video also contained visible platform branding, and I renamed
the files using the word "SYNTHETIC." The repository included a
prominent disclosure explaining that the media was AI-generated.

These measures provide context.

However, the creator cannot completely control context after an
artifact leaves its original environment.

Imagine that someone downloads my D-ID video.

The original repository explains exactly how it was produced, but the
person crops the video so the visible D-ID branding disappears. The
video is then uploaded elsewhere under a different filename without the
repository disclosure.

The pixels representing the presenter may remain mostly unchanged, but
the information available to the audience has changed significantly.

A viewer encountering that copy no longer has the same reason to
recognize it as synthetic.

This reveals an important limitation of disclosure.

Disclosure works best when the audience receives the artifact in the
environment intended by its creator. Reposting, cropping, editing,
screen recording, or re-encoding can separate content from the
information explaining its origin.

In Task 6, I did not test re-encoding, screen recording, or uploading
the artifacts to social platforms. I therefore cannot claim that my
labels or provenance information would survive those transformations.

That uncertainty itself is an important finding. Responsible creators
can provide disclosure, but they cannot guarantee that downstream
copies will preserve it.


### 2.4 Scale Axis

Task 6 required substantial attention for a very small number of
artifacts.

My preliminary DeeVid experiment took approximately 20–30 minutes.
Producing and reviewing the D-ID artifact took approximately 35–45
minutes, while the ElevenLabs audio required approximately 15–20
minutes.

Even with these relatively small time requirements, I manually reviewed
each output.

Now imagine a system connecting synthetic-media generation to an
automated pipeline.

Instead of producing one video, an organization produces 10,000
personalized videos.

Each recipient receives a synthetic presenter using a different script,
language, or recommendation.

At this scale, the ethical problem changes.

Human review that was practical for my Task 6 project becomes much more
difficult. If only one percent of 10,000 outputs contain a serious
problem, that still creates 100 problematic artifacts.

Scale therefore does more than increase quantity. It changes the
relationship between generation and oversight.

Synthetic-media systems can potentially produce content faster than
humans can meaningfully review it.

This suggests that responsible governance must consider not only what
an individual artifact contains but also how many artifacts are being
created, how automatically they are generated, and whether meaningful
human review remains possible.


## 3. Mitigation Landscape

No single mitigation completely resolves the risks identified above.
Instead, different safeguards address different parts of the problem.


### 3.1 Disclosure and Labeling

Disclosure is one of the simplest safeguards.

A creator can place an on-screen label on a synthetic video, include a
spoken disclosure in audio, add a watermark, use descriptive filenames,
or explain the synthetic nature of the content in accompanying text.

I used several of these techniques in Task 6.

The D-ID video contained visible platform branding. I renamed the final
files so that "SYNTHETIC" appeared in their filenames, and the GitHub
repository contained a prominent synthetic-media disclosure.

These measures are valuable because they give an audience information
before requiring sophisticated technical analysis.

However, disclosure has important limitations.

A watermark can potentially be cropped or covered. A filename changes
when someone downloads and renames a file. Repository documentation
does not accompany a video copied to another platform.

Disclosure therefore reduces ambiguity but cannot guarantee that every
future viewer will receive the disclosure.


### 3.2 Provenance and Content Credentials

Provenance attempts to answer a different question: where did this
content come from and what happened to it?

Approaches such as content credentials, cryptographic signatures,
metadata, and chain-of-custody records can provide information about an
artifact's origin.

My Task 6 experiment used a simpler provenance check.

I verified that the D-ID video contained visible platform branding and
maintained additional provenance through synthetic filenames and
repository documentation.

I deliberately did not claim that metadata survived re-encoding because
I did not test that process.

This experience showed why provenance should be layered.

Visible branding helps when it remains visible. Metadata helps when
systems preserve it. Documentation helps when audiences have access to
the original source.

None of these guarantees that provenance will survive every
transformation.

For this reason, provenance should support responsible communication
rather than being treated as proof that misuse is impossible.


### 3.3 Detection

Task 6 did not use a public automated deepfake detector.

Instead of claiming detector performance that I had not actually
tested, I documented a visible-watermark and provenance inspection.

This distinction matters.

Automated detectors can potentially provide useful evidence when the
origin of an artifact is uncertain. However, detection systems should
not automatically be treated as perfect authenticity tests.

Synthetic-media generators continue to change, compression can alter
media characteristics, and different generation methods can produce
different artifacts.

My own artifacts also demonstrated that humans perform a form of
informal detection. Repetitive facial movement, limited emotional
variation, uniform pacing, and reduced breathing made the artifacts
more suspicious under careful observation.

However, these cues were not always obvious during short exposure.

Detection is therefore best treated as one component of a broader
verification process rather than a single final authority.


### 3.4 Legal and Regulatory Approaches

Law and regulation can establish boundaries around synthetic-media use.

Different approaches can address areas such as required disclosure,
non-consensual synthetic imagery, impersonation, certain
election-related applications, and responsibilities placed on
platforms or creators.

Legal rules can establish consequences that voluntary guidelines
cannot.

However, law also has structural limitations.

Synthetic media can cross geographic boundaries almost instantly.
Technology may evolve faster than regulation, and identifying the
original creator of redistributed content may be difficult.

Legal requirements are therefore an important governance layer, but
they cannot replace technical safeguards, organizational controls, and
individual responsibility.


### 3.5 Platform Policy

Distribution platforms also influence synthetic-media risk.

Platforms can require disclosure, restrict certain manipulative uses,
provide reporting mechanisms, preserve provenance information, or
remove content that violates their rules.

Their position is important because even a highly convincing synthetic
artifact has limited social impact if it never reaches an audience.

However, written policy and effective enforcement are not identical.

Platforms operate at enormous scale. Synthetic content may be edited,
re-uploaded, or distributed faster than review systems can respond.

Platform rules therefore provide an important layer of governance but
cannot guarantee that misleading synthetic media will never circulate.


### 3.6 Professional and Organizational Norms

Organizations can establish rules before synthetic media is created.

This may be one of the most practical forms of mitigation because an
organization can control its own employees, contractors, approval
processes, and communication channels more directly than it can control
the entire internet.

Internal standards can require consent, disclosure, provenance,
documentation, factual verification, and human review.

However, organizational rules still depend on people following them.

A well-intentioned employee can misunderstand a requirement. A rushed
employee can skip a step. A malicious person can intentionally bypass
controls.

Organizational policy should therefore reduce predictable risk while
acknowledging that no written document can guarantee responsible human
behavior.


## 4. Overall Ethical Reflection

The most important lesson I carried from Task 6 into Task 7 is that
synthetic media cannot be evaluated using a single question such as,
"Was AI used?"

My Task 6 artifacts were synthetic, but they were relatively low risk.
They used a generic avatar and stock voices, communicated a
data-grounded fictional sports analysis, and were openly identified as
synthetic.

Changing only a few variables creates very different situations.

False information changes the truth relationship.

Using another person's identity changes the consent relationship.

Removing disclosure changes the audience's context.

Automating production changes the scale of possible consequences.

The technology itself matters, but governance depends heavily on the
circumstances surrounding its use.

That is why the next phase of this project translates these observations
into a policy designed for a specific organizational environment.
