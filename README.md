<!--- Licensed to the Apache Software Foundation (ASF) under one -->
<!--- or more contributor license agreements.  See the NOTICE file -->
<!--- distributed with this work for additional information -->
<!--- regarding copyright ownership.  The ASF licenses this file -->
<!--- to you under the Apache License, Version 2.0 (the -->
<!--- "License"); you may not use this file except in compliance -->
<!--- with the License.  You may obtain a copy of the License at -->

<!---   http://www.apache.org/licenses/LICENSE-2.0 -->

<!--- Unless required by applicable law or agreed to in writing, -->
<!--- software distributed under the License is distributed on an -->
<!--- "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY -->
<!--- KIND, either express or implied.  See the License for the -->
<!--- specific language governing permissions and limitations -->
<!--- under the License. -->

# TVM RFCs

## Table of Contents
[Table of Contents]: #table-of-contents

  - [Table of Contents]
  - [What is an RFC]
  - [RFC Audience]
  - [RFC Workflow]
  - [References]
  - [About TVM]
  - [License]
  - [Contribute to TVM]

## What is an RFC?
[What is an RFC]: #what-is-an-rfc

An RFC is a “Request for Change” to the TVM project. It is a design document
that describes a new feature, enhancement, or process to the TVM project. RFCs
should be the primary mechanism for proposing major features and changes. The
author of the RFC is responsible for the discussion of the change, and for
organizing the work around it. RFCs are text files, stored in the [Apache TVM
RFC repository](https://github.com/apache/tvm-rfcs), that serve as history and
documentation of TVM features.

## RFC Audience
[RFC Audience]: #rfc-audience

The primary audience of RFCs is the TVM development community. RFCs serve as a
guide for the design and implementation of features during and after their
development. A secondary audience is general users and developers who are
interested in how and why a feature was designed and implemented.

## RFC Workflow
[RFC Workflow]: #rfc-workflow

To work on a major feature within the TVM project, an RFC must first be merged
into the TVM RFC repository as a markdown file. Once merged, the RFC is
considered to be "active" and may be implemented, with the goal of merging the
implementation into the TVM project. These are steps that should be taken in
the RFC process:

- **Community Discussion**: A need or issue is brought to the
  [discussion forum](https://discuss.tvm.apache.org). During this phase, the
  developer and user community can discuss the need for and requirements of the
  RFC.
- **Pull Request**: After or concurrent with the conversation on the discussion
  forum, a pull request is created using the format prescreibed by the
  [RFC Template](https://github.com/apache/tvm-rfcs/blob/main/0000-template.md)
    - Discussion about the details of the RFC can continue in the pull request.
	- A committer of the corresponding area will approve and merge the RFC.
      Normally the corresponding committer will become the shepherd of the
      implementation PRs.
	- RFCs are numbered consecutively based on their order of proposal,
      regardless of if they are accepted or postponed.
    - Legacy RFCs will be numbered consecutively, prefixed with the letter
      `L` to indicate it is a legacy RFC. For example, `L0001`.
	- A successful RFC will include an overview with the problem the RFC is
      attempting to address, a proposed solution that describes the design and
      implementation strategy, and a timeline for completion. Optional sections can
      include (but are not limited to) alternatives that were considered, security
      considerations, and open problems that the RFC does not solve.
	- It is expected that RFCs will change, as part of the feedback process and
      as new implementation details arise. In order to retain change and discussion
      history, changes to the RFC should not be squashed or force pushed.
    - The formal RFC may link back to the original discussion if there is
      additional context or discussion, but all of the final feature design
      must be completely described in the pull request.
- **Tracking Issue**: Upon merging a RFC, a tracking issue will be created in
  the main TVM repository, where implementors can continue sharing
  implementation details (including links to pull requests). The issue will be
  closed when the RFC is either completed or abandoned.
- **Implementation**: Work will begin on the RFC, with pull requests linking
  back to the tracking issue.  Upon completion of the RFC, the tracking issue
  will be closed with the tag "completed". It is not a requirement for the
  author of an RFC to implement it. The tracking issue will serve as the
  primary location for communication about the status of RFC implementation. If
  you are curious about who is working on an RFC, feel free to ask on the
  comment on the associated issue.
- **Changes**: It is not uncommon for design changes to be required during or
  after the initial implementation. If this is the case, the RFC should be
  updated to reflect the change. In the instance where the change is a
  significant addition rather than a simple modification, a new RFC should be
  posted with appropriate tracking issue.
- **Postponement**: An RFC may be postponed either explicitly by the parties
  responsible for implementing it, or implicitly by having no work done for a
  period of time defined by project leaders. The tracking issue for the RFC
  will be closed with the tag "postponed".
    - **Resuming an Postponed RFC**: Work on a postponed RFC may be resumed by
      a new responsible party at any time after appropriate discussion in the
      tracking issue. The issue will be reopened, and the "postponed" tag
      removed.

## References
[References]: #references

[RFC Discussion Post](https://discuss.tvm.apache.org/t/rfc-update-rfc-process/9033)

# About TVM
[About TVM]: #about-tvm

Apache TVM is a compiler stack for deep learning systems. It is designed to
close the gap between the productivity-focused deep learning frameworks, and
the performance- and efficiency-focused hardware backends. TVM works with deep
learning frameworks to provide end to end compilation to different backends.

## License
[License]: #license
© Contributors Licensed under an [Apache-2.0](LICENSE) license.

## Contribute to TVM
[Contribute to TVM]: #contribute-to-tvm
TVM adopts Apache committer model. We aim to create an open source project that
is maintained and owned by the community. Check out the
[Contributor Guide](https://tvm.apache.org/docs/contribute/).
