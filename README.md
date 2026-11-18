# SZP-Addons

Sound dimension:

    OutsideGarden

    elseif AUDIO_VERSION == "OutsideGarden" then
	-- Gentle, open-air ambient sound with minimal wall reflections
	clubReverb.DecayTime = 1.2       -- Short echo decay (sound escapes into open air)
	clubReverb.Density = 0.3         -- Low density for light, airy reflections
	clubReverb.Diffusion = 0.4       -- Soft, scattered diffusion
	clubReverb.WetLevel = -12        -- Very subtle reverb presence

	clubEQ.HighGain = 2   -- Crisp high frequencies for an open, airy feeling
	clubEQ.MidGain = -1   -- Slightly scooped mids for a smooth background mix
	clubEQ.LowGain = -3   -- Rolled-off bass since low frequencies don't trap outdoors

    Abandoned

    elseif AUDIO_VERSION == "Abandoned" then
	-- Quiet, hollow abandoned building with long echoing walls
	clubReverb.DecayTime = 4.5       -- Long, empty echo tail
	clubReverb.Density = 0.4         -- Sparse, hollow reflections
	clubReverb.Diffusion = 0.5       -- Unfiltered, raw echoes off hard surfaces
	clubReverb.WetLevel = -1         -- Higher reverb mix relative to the quiet track

	clubEQ.HighGain = -6  -- Muffles treble to sound distant and dusty
	clubEQ.MidGain = 3    -- Enhances hollow, resonant room frequencies
	clubEQ.LowGain = -4   -- Reduces deep bass so it doesn't sound full or heavy

    Lobby 

    elseif AUDIO_VERSION == "Lobby" then
	-- High-ceiling modern glass & marble lobby with crisp, bright acoustics
	clubReverb.DecayTime = 2.0       -- Clean, airy decay without getting muddy
	clubReverb.Density = 0.8         -- Smooth reflections off glass and stone
	clubReverb.Diffusion = 0.8       -- Evenly spread, upscale background wash
	clubReverb.WetLevel = -7         -- Balanced spatial presence

	clubEQ.HighGain = 2   -- Crisp treble off glass panels and tile floors
	clubEQ.MidGain = 0    -- Natural, uncolored midrange
	clubEQ.LowGain = -2   -- Light, clean low-end so ambient music stays airy

    Underground 

    elseif AUDIO_VERSION == "Underground" then
    	-- Enclosed concrete basement / tunnel with heavy low-end and dampened highs
    	clubReverb.DecayTime = 3.8       -- Heavy, lingering concrete tunnel echo
    	clubReverb.Density = 0.9         -- Thick, close-wall reflections
    	clubReverb.Diffusion = 0.45      -- Distinct, metallic/concrete slapback
    	clubReverb.WetLevel = -2         -- Strong enclosed room resonance

    	clubEQ.HighGain = -7  -- Cuts sharp highs for that muffled, subterranean feel
    	clubEQ.MidGain = 2    -- Slight boxy resonance from enclosed concrete walls
    	clubEQ.LowGain = 5    -- Boosts deep rumble and sub-bass pressure
