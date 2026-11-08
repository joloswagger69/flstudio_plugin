nwa_claim_plugin_identity(RaveStation Rvs1 "RAVE-STATION")

juce_add_plugin(RaveStation
    COMPANY_NAME "NEOWAVE AUDIO"
    VERSION ${PROJECT_VERSION}
    PLUGIN_MANUFACTURER_CODE Neow
    PLUGIN_CODE Rvs1
    FORMATS VST3 Standalone
    PRODUCT_NAME "RAVE-STATION"
    IS_SYNTH TRUE
    NEEDS_MIDI_INPUT TRUE
    NEEDS_MIDI_OUTPUT FALSE
    EDITOR_WANTS_KEYBOARD_FOCUS FALSE
    COPY_PLUGIN_AFTER_BUILD FALSE
    VST3_CATEGORIES Instrument Drum Sampler)

target_sources(RaveStation PRIVATE Source/Plugin.cpp)
target_link_libraries(RaveStation
    PRIVATE nwa_core
    PUBLIC juce::juce_recommended_config_flags juce::juce_recommended_lto_flags juce::juce_recommended_warning_flags)
