![Proof of Humanity banner](https://ipfs.kleros.io/ipfs/QmPYQxsYLRxpkJYFNaLRVBMwYd8dsFHxsYbsMooHT27c7m/poh-banner.png)

# Proof of Humanity Registry Policy

The “Proof of Humanity” curated registry of humans is a system combining social verification with video submission to create a Sybil-proof list of humans.

A common problem on the internet and in the crypto-ecosystem is the fact that users can generally create multiple accounts using different pseudonyms or addresses to receive rewards multiple times, bias votes, write multiple fake reviews, etc... This issue can be solved through the use of a Sybil-resistant identity system such as “Proof of Humanity”.

This policy serves one main purpose:

> Ensuring each entry in this registry represents a unique, living, existing human being.

## Acceptance Criteria

The criteria to be met for a submission to be accepted in this registry are the following:
- The submitter must not be already registered in the curated list.
  - For example, a submitter cannot register himself a second time in the list by using another name.
  
- The submitter must be an existing human being.
  - For example, a submitter cannot be registered if it is a computer-generated person or avatar as it would not enable the submitter to prove it is not already registered in the list.

- The submitter must be alive.
  - For example, a submitter cannot be registered if he is deceased.
  
- The submitter must provide all the elements required for the submission.
  - For example, a submitter cannot be registered if his video submission does not display his Ethereum address.

- The submitter must respect the vouchallenger removal period, as defined in the Vouchallenger section of this policy.
  
## Elements Required for Submission

Any submitter registering to the list has to provide evidence that he is compliant with the acceptance criteria. The required evidence is to be decided through Kleros governance and can be updated to take into account technological evolutions and the evolution of attack vectors.

### List of current required/optional elements and submission rules

1. **Submitter Name** - *Required*

The submitter is composed of:
  a. Name under which the submitter is known (any UTF8 characters) - Required
  b. First Name (basic latin) - Optional
  c. Last Name (basic latin) - Optional

- Field a. information: The submitter can choose any name he is usually referred by. This can be an official name (Federico Ast), a use name (Satoshi Nakamoto), a religious/monarch name (Benedict XVI), a name with the original non-latin characters (小明), a name with anglicised characters (Xiao Ming), a name with an initialized middle name (George P. Burdell), a stage name (Bob Dylan), a political name (Nicolas Sarkozy).
- Fields b. and c. may be void if the submitter does not have it. Note that middle names are not required.
- Fields b. and c. using characters other than basic latin must be transcribed to basic latin.

2. **Front-facing Submitter Picture** - *Required*

- The picture must include the face of the submitter facing the camera and the facial features must be visible.
- The picture must be in color and not contain any artificial modification to the facial features.
- The picture must be under 3MB and have a minimum resolution of 256px by 256px.
- The picture must be in the right orientation for the face to be recognized. Image rotation is not allowed.
- Face should not be covered under large piercings or masks hindering the visibility of facial features.
- Neutral, soft and natural make-up without colored lipstick, eyeliner or eyeshadows are acceptable. Any make-up product or item that significantly alters or modifies facial features is not allowed.
- Headcover not covering the internal region of the face is acceptable (For example, a hijab is acceptable for a submitter but a niqab is not).
- It can include items worn daily (ex: headscarf, turban, wig, etc) provided they do not violate the previous points. It cannot include special items worn only on special occasions that can, voluntarily or involuntarily, distract humans or algorithms from being able to detect identical faces.

3. **Short bio** - *Optional*
- A set of words describing the submitter (For example: “Cypherpunk”, “Painting Enthusiast”, “Solidity Developer”, etc…)
- This field may be left empty.

4. **Video of the submitter** - *Required*
- The user can choose to display his Ethereum address using a physical sign. The sign has to display in a readable manner the full Ethereum address of the submitter (No ENS; no ellipsis). The sign can be a screen. The submitter must show the sign in the right orientation to be read on the video. A single one of the following errors occurring once will be tolerated in the displayed address:
  - omitted character: a character is omitted from the address (e.g. “abcd” → “abd”).
  - mistaken character: a different character has been written in place of the one expected in that position (e.g. “abcd” → “ab9d”).
  - swapped adjacent characters: two characters adjacent to each other have been swapped (e.g. “abcd” → “acbd”, but not “adcb”).
  - additional character: an additional character has been inserted anywhere in the address (e.g. “abcd” → “abc0d”).
  
- The user can choose to use verbal confirmation. The user says the *address-bound phrase* when recording their video. This 15-word phrase is the result of turning the submitter's Ethereum address into base 2048 and then matching these with the BIP-039 dictionary of the same language that the user is using for the rest of the phrase. Poor accents or mispronunciations are not grounds for rejections. The verbal confirmation must be said in the same language as the rest of the phrase.
Verifying the correctness of verbal confirmation is done through the following process: Write down the words said by the submitter, in the same order they are announced. This is the *announced phrase*. Now, up to seven words can be omitted from the address-bound phrase, with the result respecting the sequential order of the remaining words. Then, separately, up to seven words can be omitted from the announced phrase, with the result also respecting the sequential order of the remaining words. Finally, if the two resulting phrases are the exact same, the verbal confirmation is successful. Otherwise, if there is no possible way of, through this process, making the two resulting phrases be the exact same, the verbal confirmation is unsuccessful. 
- The submitter must say « I certify that I am a real human and that I am not already registered in this registry ». Submitters should speak in their normal voice and should not attempt mimicking someone else’s voice. Speaking before or after the required sentence is acceptable. Poor English accents, mispronunciations, and the switch or oversight of words in that sentence are not grounds for rejections.
- As an alternative, native spanish speakers may say the phrase: "Certifico que soy una persona humana real y que no estoy actualmente en este registro". If other words or extra validation phrases are required, they must be said in Spanish as well. Casual omission of words of the phrase, or accents are not grounds for removals or challenges and rejections. Mispronunciations of the words in that phrase are. Submitters should speak in their normal voice and should not attempt mimicking someone else’s voice. Speaking before or after the required sentence is acceptable.
- Video submissions must follow all of the following requirements:
  * at most 2 minutes long,
  * in the video/webm, video/MP4, video/avi or video/mov format,
  * vertical (portrait), horizontal (landscape) or square,
  
  and follow these minimum size requirements:
  * Minimum height: equal to or higher than 352 pixels
  * Minimum width: equal to or higher than 352 pixels

- Lighting conditions and recording device quality should be sufficient to discern facial features and characters composing the Ethereum address displayed.
- The quality of the audio should be high enough such that the speaker can be understood clearly. Small background noises are acceptable as long as they don’t prevent a clear understanding of the speaker.
- The face of the submitter should follow the requirements of section 2.

None of the provided information should be purposely offensive or hateful (ex: a painted Hindu swastika is acceptable for picture 2., even if it can be offensive to some people unfamiliar with its meaning, but « I hate Jews » as a bio is not).

## Challenge Types

In order to curate this registry, any user can challenge submissions in “Pending Registration” state that they deem non-compliant with the above-cited acceptance criteria. A user challenging a pending submission needs to specify a challenge type. A challenge can be rejected if the challenge type specified is incorrect.
A challenge must be ruled as "Refuse to arbitrate" in the case that it is the result of a vouch from a human previously removed due to vouchallenging. 

The challenges types are the following:

- Duplicate: The submitter is already registered in the list.
  - The challenger has to point to the identity already registered or to a duplicate submission. If someone tries to register multiple times simultaneously, all submissions are to be rejected.

- Does not exist: The submitter does not exist.
  - The challenger can demonstrate that the submitter is not an existing human being.

- Incorrect submission: The elements required for the submission are incorrect.
  - This kind of challenge does not claim that the submitter is trying an attack, but just that the submission does not comply with the submission rules.
  
- Deceased: The submitter has existed but does not exist anymore.
  - The challenger can provide evidence that the submitter is dead such as a death certificate, an obituary, or public records.
  - The challenged submitter can provide a video of himself reading a recent block hash. Submitters not able to give recent proof of life are to be considered deceased.
  
## Removal Request

A request to remove a submission in “Registered” state from the list can be made at any time by anyone submitting a deposit.

The removal requester has to either:

- Provide evidence that the above-cited acceptance criteria are not fulfilled by the submission.
  - Example: Send the following removal request
    - Evidence name: This user video is a deep-fake
    - Evidence description: You will find in the attached file an analysis report proving that this video is deep-faked.


- Or provide evidence that he is the submitter and wants to voluntarily remove his submission.
  - Example 1: Send a removal request from the same address as the submitter.
    - Evidence Name: Self-removal of submission
    - Evidence Description: I am the submitter as proven by my address and I want to remove this submission.
  - Example 2: Send a removal request from a different address than the submitter.
    - Evidence Name: Self-removal of submission
    - Evidence Description: I am the submitter and I want to remove this submission. The video attached is a recording of myself saying the sentence “I want to remove my own submission from the Proof of Humanity registry.”

- Or provide evidence that the submitter is a vouchallenger in accordance to the Vouchallengers Section (HIP-57) below. 

## Vouchallengers Section (HIP-58)

### 1. Definition
For the purposes of this document, a **vouchallenge** is a vouch performed on a profile that results in that profile being challenged for any challenge type. 

The **vouchallenger** is the profile that performs a vouchallenge, AND:
- A profile that did not perform a whitehat vouchallenge according to sub-section 1.2. of this Section, AND
- A profile that exceeds or equals the `max_vouchallenge_ratio`. The ratio is calculated as `vouches_wtih_incorrect_submissions / total_vouches`, AND 
- A profile that has vouched at least `initial_vouchallenge_threshold` that ended in any type of challenge, OR
- A profile that after being already removed for being a vouchallenger, makes at least `repeated_vouchallenge_threshold=1` vouchallenges, OR
- A profile that was bribed to perform a single vouchallenge according to sub-section 1.3 of this Section.

Parameters to consider: 
`max_vouchallenge_ratio = 1/2`
`initial_vouchallenge_threshold=2`, 
`repeated_vouchallenge_threshold=1`

#### 1.1. Retroactivity

This section is not retroactive to profiles that performed vouchallenges in the past that cross the initial_vouchallenge_threshold. However, if a previously active vouchallenger performs a new vouchallenge, and it is above the `repeated_vouchallenge_threshold` it will be considered a vouchallenger and will be removed.

#### 1.2. Whitehat vouchallenge

In the case the deposit is returned to the challenged person from a vouchallenger that meets the criteria of section 1, that vouchallenge is not considered for the total count. The total deposit fund must be returned before the end of the evidence period of the removal request challenge of that same vouchallenge. 

#### 1.3. Bribed vouchallenge

If there is proof (transaction records) that a vouchallenge is performed by a wallet/profile that received funds or tokens from another wallet/profile or a standalone wallet, the total count of vouchallenges is added to both wallets. NOTE: Vouchallenger counts CAN apply to unregistered ethereum wallets.

Proof applies for wallets directly or indirectly connected to other wallets by funding/being funded in the last 6 months. 

### 2. Inadmissibility period

A vouchallenger cannot be admitted back into the registry within its inadmissibility period. It is calculated as inadmissibility_period = 

`inadmissibility_period = base_period*(times_removed)`

That `base_period` is 120 days (4 months). A vouchallenger that continues vouchallenging after a removal will be removed again folowing sub-section 1 of this Section. The next inadmissible periods will be calculated considering the number of `times_removed` from the registry due to a vouchallenge.

### 3. Case Examples

* A recently registered profile that vouches its first profile that ends in challenge. 
	* Not a vouchallenger since the minimum of vouchallenges is 2
* A profile that has 24 vouchallenges but 340 total vouches
	* The ratio 24/340 is 0.07, so not a vouchallenger
* A profile that has 2 vouchallenges and 3 total vouches
	* The ratio = 2/3, so it is a vouchallenger
* A profile that was previously removed as a vouchallenger and after re-registering, it vouchallenges again
	* The profile is a vouchallenger
* A person that attemps re-registering the day after they get removed as a vouchallenger
	* The profile is challengeable and whoever challenges it gets the vouchallenger deposit.
* A profile that has a ratio of 0.87 before the implementation of this hip, and then performs a challenge:
	* Sub-section 1.1 applies, profile is a vouchallenger
* A profile that is being requested a removal for vouchallenging, but returns the deposit to the address of the vouchallenged
	* Not a vouchallenger, and the vouchallenged is not added to total vouchallenges.
* A profile that it is proven that he received funds from a wallet tied with transactions from a known or reported vouchallenger address (registered or not).
	* A vouchallenger, no matter the ratio according to subsection 1.3.

