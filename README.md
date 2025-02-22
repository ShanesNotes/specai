# Specai
Healthcare AI Agent - with executable task functions like real-time monitoring and EHR documentation. Also with modular chatbot integration for bedside assistive clinical resource

A Rust-based AI agent optimizing nurse workflows and patient care, built with the Rig framework (from ARC) and ARC on Solana, inspired by Piotr Ostr’s (@piotrostr) Listen toolkit (https://github.com/piotrostr/listen). SpecAI is a "Healthcare Leatherman" blending simulated healthcare expertise with modular chatbot capabilities.

## Features
- **Healthcare Expertise**: workflows, data validation, troubleshooting (Veteran 14+ years Critical Care RN expertise).
- **Modularity**: Rig’s AgentBuilder (from ARC) and Listen’s CLI toolkit (@piotrostr).
- **Security**: ARC blockchain logging with SHA-256; Epic FHIR API simulation with OAuth 2.0 placeholder.
- **Documentation**: Simulated immutable trails on Solana/Epic (requires live integration).
- **Chatbot**: Voice-enabled bedside clinical assistant (e.g., “Tell me about your day”).

**Note**: APIs (Epic FHIR, Philips IntelliVue, voice) are simulated using open-source data (OpenEMR, Tidepool). Live functionality requires corporate approval and integration.

## ARC Handshakes Proposal
SpecAI enhances healthcare with a “Leatherman” approach, inspired by @piotrostr’s Listen. We aim to revolutionize nurse efficiency and patient comfort, integrating ARC for secure logging and tokenomics (SpecAI token). Submission planned for May 1, 2025.

## Architecture Flowchart
Below is a flowchart of SpecAI’s architecture, inspired by @piotrostr’s Listen repository:
+----------------+ +----------------+ +----------------+
| Rig Agent Kit | ----> | Workflow | ----> | Data Service |
| (AgentBuilder)| | Pipeline | | (Simulated |
| - Nurse Mode | | - Task | | Vitals, EHR) |
| - Patient Mode| | Prioritization| | |
| - Chatbot Mode| | - IV Compat | +----------------+
+----------------+ +----------------+ |
         | | v
         v v +----------------+
+----------------+ +----------------+ | Solana ARC |
| Tools | | Epic FHIR API | --> | - Blockchain |
| - VitalsCheck | <---->| - Simulated | | Logging |
| - Custom Tools| | Logs/Data | | - SpecAI Token|
+----------------+ +----------------+ +----------------+


- **Rig Agent Kit**: Configures modes using Rig’s AgentBuilder (from ARC, https://github.com/0xPlaygrounds/rig).
- **Workflow Pipeline**: Prioritizes tasks, inspired by Listen’s Trading Engine (@piotrostr).
- **Data Service**: Streams simulated vitals (Tidepool) and EHR data (OpenEMR).
- **Epic FHIR API**: Simulated logs/data (requires live integration).
- **Solana ARC**: Blockchain logging with SHA-256, influenced by Listen (@piotrostr).

## Setup
1. **Clone Repo**: `git clone https://github.com/yourusername/SpecAI-Agent.git`
2. **Install Dependencies**: `cd SpecAI-Agent && cargo build --release`
3. **Run Examples**:
   - Healthcare: `cargo run --release -- interact "How am I doing?" --voice`
   - Chatbot: `cargo run --release -- interact "Tell me about your day" --voice`
   - Monitor: `cargo run --release -- monitor-vitals P001`

## Roadmap
- **March 15, 2025**: Rust executable with Rig and Listen-inspired CLI (@piotrostr).
- **May 1, 2025**: Handshakes submission with demo.
- **July 1, 2025**: Initial launch with SpecAI token.

## Contributing
See `CONTRIBUTING.md`. Join “SpecAI Handshakes” to enhance this toolkit!

## Credit
- **(@piotrostr)**: Listen’s CLI, pipeline, and Solana inspiration (https://github.com/piotrostr/listen).
- **ARC Team**: Rig framework (https://github.com/0xPlaygrounds/rig).

## License
Apache 2.0
