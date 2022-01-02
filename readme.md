This is a mirror of: https://forge.codesys.com/git/lib,cobolt,binaries.git/

This roadmap is subjected to change without prior notice. No liabilities shall be taken! Completed milestones are clearly marked below;

v2.0.0.0 Standard version: Full-spec Edge, Device and Host implementation for CODESYS based industrial controllers

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
