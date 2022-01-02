All relevant info about this project can be found on: https://forge.codesys.com/lib/cobolt/

This is a binaries mirror of: https://forge.codesys.com/git/lib,cobolt,binaries.git/

Designed by the co-author of MQTT, Arlen Nipper, Sparkplug™ is designed to fit "on top" of regular MQTT. In 1999, when MQTT was invented, it was originally meant for SCADA systems and left out all specifications on how topics and payloads should be structured and how devices should behave. This allowed regular MQTT to be used in different industries, but lacked any standard topic or dataformat.

Sparkplug™ now fills this gap and provides a vendor-neutral specification for the data formats, topic structures, state management, and how topologies should be structured in IIoT scenarios. This way, Sparkplug™ adds several smart features on top of regular MQTT, resulting in a "Sparkplug™ enhanced MQTT". A flexible architecture which allows you to auto-discover edge nodes, devices and their metrics (data & metadata) as devices and applications can be added and removed anytime without affecting the system as a whole. Report by Exception (RBE) saves bandwidth, memory and computational power on the producer and the consumers of data. Last but not least, your data can be delivered securely via the latest industry strength security specifications and with rich meta-data for added context. 

BY DOWNLOADING AND USAGE OF THESE LIBRARIES YOU ABIDE BY THE MIT LICENSE

This roadmap is subjected to change without prior notice. No liabilities shall be taken! Completed milestones are clearly marked below;
v2.0.0.0 Standard version: Full-spec stable Edge, Device and a proof of concept Host implementation for CODESYS based industrial controllers

    All Datatype Metrics supported,
    Device support, acts as a digital representation of a physical device sending metrics,
    Receive Server Commands, setpoints etc, (xCMD),
    Bind multiple Devices to Edge,
    Machine to Machine communication,
    Seperate libraries:
        co⚡e: Sparkplug™ MQTT Stack - Contains a common basis for Edge and Host solutions,
        co⚡e: Sparkplug™ MQTT Edge - Contains Edge and Device solution,
        co⚡e: Sparkplug™ MQTT Host - Contains Primary Host solution,
        co🔗e: A Linked List Solution.
    Support for Metric Properties,
        Read Only Property (Mandatory Included),
        Any User Defined Property,
        Ignition verified,
    Support for Aliases,
        Edge / Device send server xBIRTH & xDATA via Alias
        Edge / Device receive server xCMD via Alias
        Ignition verified
    Template i.e. Edge / Device complex variables (nested structs) support,
        Edge / Device send server xBIRTH Template support,
        Edge / Device send server xDATA Template support,
        Edge / Device receive server xCMD Template support,
        Ignition verified
    WebSockets support,
        HTTP ( ws://...:8080 ) verified,
        HTTPS through TLS Support ( wss://...:8083 ) Experimental,
        Proxy Settings (Server Address, Port, Username, Password)
    Edge Publishes Properties like
        ABOUT (mandatory),
        Compiler version,
        Runtime Version,
        NIC (Up to 8 supported) name, MAC & IP addresses,
        OS version, etc,
        Extended Info Opt-Out,
        Ignition verified
    CODESYS based Primary Host Node implementation,
        Server receive Edge / Device xBIRTH,
        Server receive Edge / Device xDATA,
        Server receive Edge / Device xCMD,
        Server receive Edge / Device xDEATH & LWT -> Data becomes STALE
        Server send Edge / device xCMD (DATA)
        Strict enforcement of SEQ / BDSEQ check,
        Server sends Edge REBIRTH to Edge or Device,
        WebSocket support,
        Metric property support,
        Alias Support.
