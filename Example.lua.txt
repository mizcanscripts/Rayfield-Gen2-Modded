local Rayfield = loadstring(readfile("Rayfield.luau"))()

task.wait(2)

-- Rayfield:AddTheme(properties) registers a new theme by name. Any key you leave out falls
-- back to the Dark theme's default (same rule as passing a table straight to ChangeTheme).
-- Once registered it shows up automatically in the built-in Settings tab's Theme dropdown,
-- and can be selected as the initial CreateWindow Theme below, both by this exact Name string.
-- Every property below is optional — this lists all of them together as a full reference.
-- Color3 on a gradient-capable key (noted below) is auto-wrapped into a solid ColorSequence.
Rayfield:AddTheme({
    Name = "Sakura Dusk",

    CornerRoundness     = UDim.new(0, 24),
    ElementCornerRadius = UDim.new(0, 14),
    PillCornerRadius    = UDim.new(1, 0),

    WindowColor = ColorSequence.new({
        ColorSequenceKeypoint.new(0,      Color3.fromRGB(255, 248, 250)),
        ColorSequenceKeypoint.new(0.5,    Color3.fromRGB(252, 240, 245)),
        ColorSequenceKeypoint.new(0.9999, Color3.fromRGB(250, 232, 240)),
        ColorSequenceKeypoint.new(1,      Color3.fromRGB(248, 225, 236)),
    }),
    ShadowColor = Color3.fromRGB(210, 175, 190),

    ElementGradient                = Color3.fromRGB(255, 252, 254),
    ElementStroke                  = Color3.fromRGB(240, 200, 218),
    ElementStrokeGradient          = Color3.fromRGB(230, 185, 205),
    ElementStrokeHover             = Color3.fromRGB(220, 90, 130),
    ElementTransparency            = 0,
    ElementStrokeTransparency      = 0,
    ElementStrokeHoverTransparency = 0,
    ElementTextHoverColor          = Color3.fromRGB(100, 30, 55),

    TabColor      = Color3.fromRGB(130, 40, 70),
    TabBackground = Color3.fromRGB(248, 232, 240),
    TabStroke     = Color3.fromRGB(210, 130, 160),

    SliderBackground      = Color3.fromRGB(252, 238, 245),
    SliderBackgroundHover = Color3.fromRGB(248, 228, 238),
    SliderProgress        = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(215, 80, 120)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(240, 140, 170)),
    }),
    SliderStroke          = Color3.fromRGB(210, 160, 180),
    SliderHandle          = Color3.fromRGB(215, 80, 120),

    ToggleTrack               = Color3.fromRGB(215, 80, 120),
    ToggleTrackTransparency   = 0.6,
    ToggleKnobOff             = Color3.fromRGB(195, 150, 170),
    ToggleKnobOffTransparency = 0.3,
    DarkToggleOverlay         = false,

    FieldBackground   = Color3.fromRGB(255, 255, 255),
    FieldTransparency = 0.0,
    FieldGlow         = Color3.fromRGB(215, 80, 120),
    PlaceholderColor  = Color3.fromRGB(185, 145, 162),
    SurfaceStroke     = Color3.fromRGB(220, 185, 200),

    NeutralButton       = Color3.fromRGB(245, 228, 236),
    NeutralButtonHover  = Color3.fromRGB(238, 215, 226),
    NeutralButtonStroke = Color3.fromRGB(210, 165, 185),

    ContentColor = Color3.fromRGB(130, 85, 105),
    TitlingColor = Color3.fromRGB(90, 30, 55),
    ActionColor  = Color3.fromRGB(180, 70, 105),

    AccentColor  = Color3.fromRGB(215, 80, 120),
    AccentStroke = Color3.fromRGB(240, 130, 162),
    AccentGlow   = 0.3,

    StatBackground    = Color3.fromRGB(250, 235, 242),
    DropdownHighlight = Color3.fromRGB(215, 80, 120),

    ErrorColor       = Color3.fromRGB(200, 50, 50),
    ErrorStrokeColor = Color3.fromRGB(230, 85, 85),

    Font      = Font.new("rbxasset://fonts/families/Nunito.json", Enum.FontWeight.Medium, Enum.FontStyle.Normal),
    TitleFont = Font.new("rbxasset://fonts/families/Nunito.json", Enum.FontWeight.Bold,   Enum.FontStyle.Normal),

    LiveAnimation = true,
})

Rayfield:AddTheme({
    Name = "Arctic Circuit",

    CornerRoundness     = UDim.new(0, 12),
    ElementCornerRadius = UDim.new(0, 7),
    PillCornerRadius    = UDim.new(1, 0),

    WindowColor = ColorSequence.new({
        ColorSequenceKeypoint.new(0,      Color3.fromRGB(240, 248, 255)),
        ColorSequenceKeypoint.new(0.5,    Color3.fromRGB(232, 242, 252)),
        ColorSequenceKeypoint.new(0.9999, Color3.fromRGB(224, 236, 250)),
        ColorSequenceKeypoint.new(1,      Color3.fromRGB(216, 230, 248)),
    }),
    ShadowColor = Color3.fromRGB(170, 195, 225),

    ElementGradient                = Color3.fromRGB(248, 252, 255),
    ElementStroke                  = Color3.fromRGB(190, 215, 240),
    ElementStrokeGradient          = Color3.fromRGB(170, 200, 232),
    ElementStrokeHover             = Color3.fromRGB(55, 140, 210),
    ElementTransparency            = 0,
    ElementStrokeTransparency      = 0,
    ElementStrokeHoverTransparency = 0,
    ElementTextHoverColor          = Color3.fromRGB(15, 60, 110),

    TabColor      = Color3.fromRGB(20, 75, 140),
    TabBackground = Color3.fromRGB(222, 236, 252),
    TabStroke     = Color3.fromRGB(80, 155, 220),

    SliderBackground      = Color3.fromRGB(232, 244, 255),
    SliderBackgroundHover = Color3.fromRGB(218, 234, 250),
    SliderProgress        = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(50, 120, 200)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(90, 165, 235)),
    }),
    SliderStroke          = Color3.fromRGB(150, 190, 225),
    SliderHandle          = Color3.fromRGB(50, 120, 200),

    ToggleTrack               = Color3.fromRGB(55, 130, 205),
    ToggleTrackTransparency   = 0.6,
    ToggleKnobOff             = Color3.fromRGB(150, 185, 218),
    ToggleKnobOffTransparency = 0.3,
    DarkToggleOverlay         = false,

    FieldBackground   = Color3.fromRGB(255, 255, 255),
    FieldTransparency = 0.0,
    FieldGlow         = Color3.fromRGB(55, 130, 205),
    PlaceholderColor  = Color3.fromRGB(145, 175, 205),
    SurfaceStroke     = Color3.fromRGB(175, 205, 232),

    NeutralButton       = Color3.fromRGB(228, 240, 252),
    NeutralButtonHover  = Color3.fromRGB(212, 228, 248),
    NeutralButtonStroke = Color3.fromRGB(165, 200, 232),

    ContentColor = Color3.fromRGB(65, 100, 145),
    TitlingColor = Color3.fromRGB(18, 55, 105),
    ActionColor  = Color3.fromRGB(45, 110, 185),

    AccentColor  = Color3.fromRGB(50, 120, 200),
    AccentStroke = Color3.fromRGB(90, 158, 228),
    AccentGlow   = 0.25,

    StatBackground    = Color3.fromRGB(225, 238, 252),
    DropdownHighlight = Color3.fromRGB(50, 120, 200),

    ErrorColor       = Color3.fromRGB(205, 50, 50),
    ErrorStrokeColor = Color3.fromRGB(235, 80, 80),

    Font      = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Medium, Enum.FontStyle.Normal),
    TitleFont = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Bold,   Enum.FontStyle.Normal),

    LiveAnimation = false,
})

Rayfield:AddTheme({
    Name = "Inferno Obsidian",

    CornerRoundness     = UDim.new(0, 14),
    ElementCornerRadius = UDim.new(0, 8),
    PillCornerRadius    = UDim.new(0, 8),

    WindowColor = ColorSequence.new({
        ColorSequenceKeypoint.new(0,      Color3.fromRGB(8,  6,  4)),
        ColorSequenceKeypoint.new(0.5,    Color3.fromRGB(12, 9,  5)),
        ColorSequenceKeypoint.new(0.9999, Color3.fromRGB(16, 11, 6)),
        ColorSequenceKeypoint.new(1,      Color3.fromRGB(20, 14, 7)),
    }),
    ShadowColor = Color3.fromRGB(3, 2, 1),

    ElementGradient                = Color3.fromRGB(24, 16, 8),
    ElementStroke                  = Color3.fromRGB(65, 40, 15),
    ElementStrokeGradient          = Color3.fromRGB(90, 55, 20),
    ElementStrokeHover             = Color3.fromRGB(240, 140, 30),
    ElementTransparency            = 0,
    ElementStrokeTransparency      = 0,
    ElementStrokeHoverTransparency = 0,
    ElementTextHoverColor          = Color3.fromRGB(255, 245, 225),

    TabColor      = Color3.fromRGB(255, 200, 100),
    TabBackground = Color3.fromRGB(18, 12, 5),
    TabStroke     = Color3.fromRGB(180, 95, 15),

    SliderBackground      = Color3.fromRGB(22, 14, 6),
    SliderBackgroundHover = Color3.fromRGB(32, 20, 8),
    SliderProgress        = ColorSequence.new({
        ColorSequenceKeypoint.new(0,   Color3.fromRGB(185, 80,  10)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(220, 120, 15)),
        ColorSequenceKeypoint.new(1,   Color3.fromRGB(250, 170, 40)),
    }),
    SliderStroke          = Color3.fromRGB(130, 70, 18),
    SliderHandle          = Color3.fromRGB(240, 145, 30),

    ToggleTrack               = Color3.fromRGB(35, 20, 6),
    ToggleTrackTransparency   = 0.4,
    ToggleKnobOff             = Color3.fromRGB(110, 65, 20),
    ToggleKnobOffTransparency = 0.4,
    DarkToggleOverlay         = true,

    FieldBackground   = Color3.fromRGB(240, 160, 60),
    FieldTransparency = 0.92,
    FieldGlow         = Color3.fromRGB(240, 130, 20),
    PlaceholderColor  = Color3.fromRGB(140, 90, 40),
    SurfaceStroke     = Color3.fromRGB(110, 60, 15),

    NeutralButton       = Color3.fromRGB(30, 18, 8),
    NeutralButtonHover  = Color3.fromRGB(44, 26, 10),
    NeutralButtonStroke = Color3.fromRGB(95, 52, 16),

    ContentColor = Color3.fromRGB(185, 140, 85),
    TitlingColor = Color3.fromRGB(245, 200, 115),
    ActionColor  = Color3.fromRGB(240, 155, 50),

    AccentColor  = Color3.fromRGB(230, 120, 20),
    AccentStroke = Color3.fromRGB(250, 168, 60),
    AccentGlow   = 0.5,

    StatBackground    = Color3.fromRGB(14, 8, 3),
    DropdownHighlight = Color3.fromRGB(230, 120, 20),

    ErrorColor       = Color3.fromRGB(240, 55, 55),
    ErrorStrokeColor = Color3.fromRGB(255, 90, 90),

    Font      = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Medium,    Enum.FontStyle.Normal),
    TitleFont = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.ExtraBold, Enum.FontStyle.Normal),

    LiveAnimation = true,
})

local window = Rayfield:CreateWindow({ --[[
    name / title        : window title (required, use " " for blank)
    subtitle / subtext  : small text under the title
    sidebarLayout       : true = sidebar rail | false = top strip (default false)
    Size                : UDim2
    Font                : Enum.Font
    Theme / theme / Themes / themes :
        "Dark" | "Blood Red" | "Amethyst" | "Rose" | "Frost" |
        "Cobalt" | "Ember" | "Gold" | "Midnight" | any name registered via Rayfield:AddTheme

    [Special]
    OpenButton.Title    : collapsed-pill label (default "RayField")
    OpenButton.Subtitle : collapsed-pill sublabel
    OpenButton.Icons    : collapsed-pill icon asset id
    UserInfo.Title      : sidebar avatar chip name
    UserInfo.Icons      : sidebar avatar chip image
    configuration.setFolder  : folder path for .json config files
    configuration.autoSave   : auto-save flags on every change
    configuration.autoLoad   : auto-load on window open
    appearance.setFolder     : folder for Options.json theme/font/transparency file
]]
    title         = "Example",
    subtitle      = "RayField Plus++",
    sidebarLayout = true, -- sidebar rail on the left; set false for a top nav strip instead

    Size  = UDim2.fromOffset(640, 640),
    Font  = Enum.Font.Gotham,
    Theme = "Midnight",

    OpenButton = { -- the small pill shown when the window is hidden
        Title    = "Plutonium",
        Subtitle = "Tap to open",
        Icons    = "rbxassetid://120122773078069",
    },

    configuration = {
        autoSave  = true,               -- every flag change is written to disk automatically
        setFolder = "Plutonium/Config", -- subfolder inside the executor workspace folder
    },

    appearance = {
        setFolder = "Plutonium", -- saves theme + font + transparency to Plutonium/Options.json
    },
})

-- CreateTab: every tab becomes one page in the sidebar (or top strip).
-- icon accepts a numeric Roblox asset id OR an icon-pack string like "lucide/home".
local home   = window:Tab({ name = "Home",   icon = 93364949241311  })
local combat = window:Tab({ name = "Combat", icon = 84750991656135  })
local fields = window:Tab({ name = "Fields", icon = 100604009889706 })
local stats  = window:Tab({ name = "Stats",  icon = 85925158736685  })
local layout = window:Tab({ name = "Layout", icon = 84750991656135  })
local blobman = window:Tab({ name = "Blobmans", icon = "rbxassetid://111081193991484" })

-- =============================================
-- Auto Update Profile: Greeting + Clock
-- =============================================

local RunService = game:GetService("RunService")
local lastSecond = -1

local function getGreeting(hour)
    if hour >= 5 and hour < 12 then
        return "Good Morning"
    elseif hour >= 12 and hour < 18 then
        return "Good Afternoon"
    elseif hour >= 18 and hour < 21 then
        return "Good Evening"
    else
        return "Good Night"
    end
end

window:Connect(RunService.Heartbeat, function()
    local now = math.floor(tick())
    if now == lastSecond then return end
    lastSecond = now

    local hour = tonumber(os.date("%H"))
    window:SetProfile(getGreeting(hour) .. " — " .. os.date("%H:%M:%S"))
end)

-- CreateSection: visual label that groups the controls below it in the scroll list.
home:Section({ name = "Gameplay" })

-- CreateToggle: on/off switch. value = starting state; callback fires every time the user flips it.
-- Returns a Toggle object with :Set(bool), :Lock(reason?), :Unlock(), :IsLocked().
home:Toggle({
    name     = "Auto Sprint",
    value    = true,
    callback = function(value) print("Auto Sprint:", value) end,
})

-- description adds a second line of smaller text below the control name.
home:Toggle({
    name        = "Reduced Motion",
    description = "Disables screen shake and camera effects.",
    callback    = function(value) print("Reduced Motion:", value) end,
})

-- CreateSlider: draggable range picker. range = {min, max}; increment = step size; suffix = unit label.
-- callback receives (currentValue, isDragging) — isDragging is true while the thumb is held.
home:Slider({
    name      = "Field of View",
    range     = { 70, 120 },
    increment = 1,
    value     = 90,
    suffix    = "°",
    callback  = function(value) workspace.CurrentCamera.FieldOfView = value end,
})

-- CreateSwitch is a plain alias for CreateToggle — same widget, same options, same return type.
home:Switch({ name = "Auto Loot", value = false, callback = function(value) print("Auto Loot:", value) end })

home:Section({ name = "Interface" })

-- A Toggle with no callback is still valid — useful as a pure saved flag read later via window.Flags.
home:Toggle({ name = "Show FPS Counter" })

-- CreateDropdown: single-select by default. options = list of strings; value = default selection.
-- Returns a Dropdown with :Set(value), :Refresh(newOptions), :Add(option), :Remove(option).
home:Dropdown({
    name     = "Quality",
    options  = { "Low", "Medium", "High", "Ultra" },
    value    = "High",
    callback = function(value) print("Quality:", value) end,
})

home:Section({ name = "Feedback" })

-- CreateButton: a tappable row that fires callback on press. icon is optional decoration.
-- The returned Button has :Lock(reason?) / :Unlock() to disable/enable it programmatically.
home:Button({
    name     = "Send Notification",
    icon     = 93364949241311,
    callback = function()
        -- window:Notify shows a floating card (top-right). duration defaults to ~5 s.
        window:Notify({
            title   = "Auto-saved",
            content = "Your configuration was saved.",
            icon    = 125823673784681,
        })
    end,
})

home:Button({
    name     = "Send Toast",
    icon     = 125823673784681,
    callback = function()
        -- window:Toast is a compact, auto-dismissing banner (lighter than Notify).
        -- Extra props: subtitle, subtitleAbove, avatar (userId), minWidth, duration, position ("Top"|"Bottom").
        window:Toast({ title = "Saved", icon = 125823673784681 })
    end,
})

home:Button({
    name     = "Open Popup",
    icon     = 83277910885129,
    callback = function()
        -- window:Popup is a modal dialog. options[] can have style = "danger" for a red button.
        -- Popup also supports boxes = { {title, description, icon} } for info panels inside it.
        -- Returns a Popup object with :Close() to dismiss it from code.
        window:Popup({
            title   = "Reset everything?",
            content = "This clears every saved value. You can't undo it.",
            icon    = 83277910885129,
            options = {
                { text = "Cancel" },
                { text = "Reset", style = "danger" },
            },
        })
    end,
})

combat:Section({ name = "Aiming" })
combat:Toggle({ name = "Aimbot", value = true })
combat:Slider({ name = "Smoothness", range = { 0, 100 }, value = 40, suffix = "%" })

-- multiSelect = true lets the user pick more than one option at once.
-- value can then be a table of strings. placeholder shows when nothing is selected.
-- callback receives a table (multiSelect) or a single string (single-select).
combat:Dropdown({
    name        = "Modules",
    description = "Pick any combination of modules to load.",
    multiSelect = true,
    options     = { "Aimbot", "ESP", "Triggerbot", "Fly" },
    value       = { "ESP" }, -- pre-select ESP on load
    placeholder = "None selected",
})

fields:Section({ name = "Setup" })

-- CreateInput: single-line text box. placeholder shows when empty.
-- Returns an Input with :Set(text) and :Lock() / :Unlock().
fields:Input({ name = "Player Name", placeholder = "Enter a name" })

-- numeric = true rejects non-digit characters while typing.
-- clearOnFocus = true wipes the box when the user taps into it (useful for default-hint patterns).
-- callback fires on blur (focus lost) or when the user presses Enter.
fields:Input({
    name        = "Max Players",
    description = "Numeric only, commits on blur or Enter.",
    numeric     = true,
    value       = "16",
})

-- CreateKeybind: key binding picker. value = default key; stored as Enum.KeyCode.
-- isMenuToggle = true makes this key also hide/show the window (overrides the built-in setting).
fields:Keybind({ name = "Sprint", value = Enum.KeyCode.LeftShift })

-- hold = true makes the callback fire with true while held and false on release, instead of toggling.
-- holdThreshold (seconds) sets how long before "held" fires.
-- onChanged fires whenever the user picks a new key (separate from the hold callback).
fields:Keybind({
    name     = "Zoom",
    value    = Enum.KeyCode.C,
    hold     = true,
    callback = function(holding) print("Zoom:", holding) end,
})

-- isMenuToggle = true makes this bind ALSO show/hide the whole window in addition to
-- whatever its own callback does, effectively replacing the window's default hide key.
fields:Keybind({
    name         = "Menu Key",
    value        = Enum.KeyCode.RightControl,
    isMenuToggle = true,
})

-- CreateColorPicker: shows a color wheel. color = Color3 default; alpha = 0..1 opacity default.
-- callback receives (Color3, alpha). :Set(color) accepts a Color3 or hex string like "#ff0000".
-- :SetAlpha(number) changes only the opacity without touching the hue.
fields:ColorPicker({
    name  = "Highlight",
    color = Color3.fromRGB(96, 205, 255),
    alpha = 1,
})

stats:Section({ name = "Session" })

-- CreateStat: a read-only numeric display. prefix/suffix wrap the number; value = starting number.
-- :Set(n) updates the displayed number (animates if numberEasing is true in props).
-- :ResetBaseline(n?) resets the delta-change indicator; pass nil to use the current value.
-- compact = true shortens large numbers (e.g. 12400 → 12.4 K). changeMode shows a +/- delta chip.
local revenue = stats:Stat({ name = "Revenue", prefix = "$",      value = 12400 })
local kills   = stats:Stat({ name = "Kills",   suffix = " kills", value = 128   })

stats:Button({
    name     = "Simulate Round",
    callback = function()
        revenue:Set(revenue.value + math.random(500, 3000)) -- .value holds the current number
        kills:Set(kills.value   + math.random(1, 20))
    end,
})

layout:Section({ name = "Loadout" })

-- CreateGroup: an invisible row container. Nest groups to build grid/column layouts.
-- direction = "column" stacks children vertically inside the group; default is horizontal (row).
local grid        = layout:Group()
local leftColumn  = grid:Group({ direction = "column" })
-- flag = explicit save key; if omitted, Rayfield derives one from the name automatically.
leftColumn:Toggle({ name = "Aimbot",     flag = "LoadoutAimbot", value = true })
leftColumn:Toggle({ name = "Triggerbot" })

local rightColumn = grid:CreateGroup({ direction = "column" })
rightColumn:Toggle({ name = "ESP",     value = true })
rightColumn:Toggle({ name = "Tracers" })

-- window:CreateSection adds a collapsible tab-group header in the sidebar (sidebarLayout only).
window:Section({ name = "Reference" })

local text = window:CreateTab({ name = "Text", icon = 100604009889706 })
text:CreateSection({ name = "Text elements" })

-- CreateText: a label element with an optional title and body. Either half can be omitted.
-- icon works the same as on any other element (asset id or icon-pack string).
text:CreateText({
    name = "Read this first",
    text = "Text carries a title, a body, or both. Either half can be left out.",
})
text:CreateText({ name = "Heading only" })           -- body omitted, only title row shown
text:CreateText({ text = "Body only — evenly padded with no room held for a title." })
text:CreateText({ name = "With an icon", text = "Any supported icon pack or Roblox asset id works here.", icon = 93364949241311 })

-- :Set(text) rewrites the body in place; :SetTitle(text) rewrites the name/title row.
local live = text:CreateText({ name = "Live text", text = "Waiting." })
text:CreateButton({ name = "Rewrite body",  callback = function() live:Set("Rewritten at " .. os.date("%H:%M:%S") .. ".") end })
text:CreateButton({ name = "Rewrite title", callback = function() live:SetTitle("Retitled") end })

text:CreateSection({ name = "Dividers" })

-- CreateDivider: a horizontal rule. text = optional centred label; spacing = extra vertical gap (px).
-- line = false removes the line entirely and only adds vertical space (blank gap element).
text:CreateDivider()
text:CreateDivider({ text = "or" })
text:CreateDivider({ text = "spaced", spacing = 24 })
text:CreateDivider({ line = false, spacing = 20 }) -- invisible spacer, no line

-- :Set(text?) swaps the centred label after creation; pass "" or nil to clear it.
local divider = text:CreateDivider()
text:CreateButton({ name = "Give divider a word", callback = function() divider:Set("added later") end })
text:CreateButton({ name = "Clear divider word",  callback = function() divider:Set("") end })

text:CreateSection({ name = "Icon packs" })
-- Icon strings follow the pattern "pack/name". Roblox asset ids (numbers) still work everywhere.
text:CreateText({ name = "lucide/palette",     icon = "lucide/palette",     text = "lucide — clean stroke icons." })
text:CreateText({ name = "gravity/home",        icon = "gravity/home",        text = "gravity — bold, rounded." })
text:CreateText({ name = "solar/sun-bold",      icon = "solar/sun-bold",      text = "solar — linear, bold, broken, outline variants." })
text:CreateText({ name = "sfsymbols/star.fill", icon = "sfsymbols/star.fill", text = "sfsymbols — Apple SF Symbols." })
text:CreateText({ name = "craft/edit",          icon = "craft/edit",          text = "craft — productivity icons." })
text:CreateText({ name = "geist/zap",           icon = "geist/zap",           text = "geist — Vercel, minimal and sharp." })
text:CreateText({ name = "hero/shield-check",   icon = "hero/shield-check",   text = "hero — Tailwind Heroicons." })
text:CreateText({ name = "gmi/search",          icon = "gmi/search",          text = "gmi — Google Material Icons." })
text:CreateText({ name = "feather/feather",     icon = "feather/feather",     text = "feather — open-source minimal." })
text:CreateText({ name = "Roblox asset id",     icon = 93364949241311,        text = "Plain numbers still work." })

local language = window:CreateTab({ name = "Language", icon = 100604009889706 })
language:CreateSection({ name = "Localization" })

local localeIds = { English = "en", ["Français"] = "fr", ["Español"] = "es", ["Deutsch"] = "de" }
-- forgetState = true makes this control never persist its value to the config file.
-- Useful for ephemeral UI state that should always reset on re-open.
language:CreateDropdown({
    name        = "Language",
    description = "Switches every localized label in place.",
    options     = { "English", "Français", "Español", "Deutsch" },
    value       = "English",
    forgetState = true,
    callback    = function(value)
        if value == "Deutsch" then
            -- RegisterTranslations: supply a table keyed by locale id, each containing
            -- a map of original string → translated string. Supports multiple locales at once.
            window:RegisterTranslations({
                de = {
                    ["Gameplay"]      = "Spiel",
                    ["Interface"]     = "Benutzeroberfläche",
                    ["Auto Sprint"]   = "Auto-Sprint",
                    ["Field of View"] = "Sichtfeld",
                    ["Player Name"]   = "Spielername",
                },
            })
        end
        -- SetLocale("en"|"fr"|"es"|"de"|…) switches all registered labels live, no reload needed.
        window:SetLocale(localeIds[value] or "en")
    end,
})

local whatsNew = window:CreateTab({ name = "What's New", icon = 93364949241311 })
whatsNew:CreateSection({ name = "Changelog" })

whatsNew:CreateText({ name = "Rich Theme Gradients",                  icon = "lucide/palette",  text = "Rose, Gold, Ember fully reworked with multi-stop ColorSequence gradients. New Midnight theme added." })
whatsNew:CreateText({ name = "SetFolder — Appearance & Config",       icon = "lucide/folder",   text = "Both managers now use setFolder. Appearance saves Theme+Font+Transparency to setFolder/Options.json." })
whatsNew:CreateText({ name = "Advanced Configuration Manager",        icon = "lucide/settings", text = "Settings tab: Saved Config dropdown, Config Name input, Set Auto Load, Load/Save/Delete buttons." })
whatsNew:CreateText({ name = "Window Transparency toggle",            icon = "lucide/eye",      text = "Built-in settings now includes a Window Transparency toggle, saved to Options.json." })
whatsNew:CreateText({ name = "Minimize state position preserved",     icon = "lucide/layout",   text = "Hiding the window no longer resets the minimize bar position." })

whatsNew:CreateSection({ name = "Progress" })

-- CreateProgress: a filled bar showing a value inside a range.
-- format(value, min, max) → string overrides the default label next to the bar.
-- showValue = true always shows the raw number even without a custom format function.
local download = whatsNew:CreateProgress({
    name   = "Download",
    range  = { 0, 100 },
    value  = 35,
    format = function(value, _, max) return string.format("%d of %d MB", value, max) end,
})

-- steps = n turns the bar into a discrete step indicator (n segments) instead of continuous.
whatsNew:CreateProgress({ name = "Setup",   steps = 5,   value = 2 })

-- indeterminate = true shows an animated looping bar when progress is unknown.
-- Call :SetIndeterminate(false) later to switch it back to a normal tracked bar.
whatsNew:CreateProgress({ name = "Syncing", text  = "Please wait", indeterminate = true })

whatsNew:CreateSlider({
    name        = "Download progress",
    range       = { 0, 100 },
    value       = 35,
    suffix      = "%",
    forgetState = true,
    callback    = function(value, dragging)
        download:Set(value)                                    -- :Set(n) moves the bar to n
        download:SetText(if dragging then "Downloading" else nil) -- :SetText(s?) overrides the label; nil restores default
    end,
})

whatsNew:CreateSection({ name = "Output" })

-- CreateConsole: a scrollable text area for logging output.
-- follow = true auto-scrolls to the bottom on every new line.
-- maxLines caps how many lines are kept (oldest are discarded when exceeded).
local console = whatsNew:CreateConsole({
    name     = "Console",
    text     = "-- output lands here", -- initial content shown on first render
    height   = 130,
    follow   = true,
    maxLines = 50,
})

-- :Append(line) adds one line to the bottom (respects maxLines / follow).
-- :Set(text) replaces the entire content at once.
-- :Get() returns the full current text as a string.
whatsNew:CreateButton({ name = "Log a line", callback = function() console:Append(string.format("[%s] player joined", os.date("%H:%M:%S"))) end })

local consoleGroup = whatsNew:CreateGroup()
-- :Copy() puts the console text onto the clipboard; returns true on success, false if no clipboard API.
consoleGroup:CreateButton({ name = "Copy",  callback = function() window:Notify({ title = if console:Copy() then "Copied" else "No clipboard here" }) end })
-- :Clear() wipes all text from the console box.
consoleGroup:CreateButton({ name = "Clear", callback = function() console:Clear() end })

whatsNew:CreateSection({ name = "Locking" })

-- :Lock(reason?) grays out the element, prevents interaction, and shows reason as a tooltip.
-- :Unlock() restores it. :IsLocked() → boolean checks current state.
-- While locked the callback never fires, even if Set() is called programmatically.
local lockable = whatsNew:CreateToggle({
    name        = "Auto Farm",
    description = "Lock this and it dims, stops taking input, never fires its callback.",
    value       = false,
    forgetState = true,
    callback    = function(state) print("never runs while locked", state) end,
})

whatsNew:CreateToggle({
    name        = "Lock Auto Farm",
    value       = false,
    forgetState = true,
    callback    = function(state)
        if state then lockable:Lock("Needs a premium key") else lockable:Unlock() end
    end,
})

local api = window:CreateTab({ name = "Window API", icon = 84750991656135 })

api:CreateSection({ name = "Theme" })

-- window:ChangeTheme(name) swaps every themed color live, no reload needed.
-- Accepts any built-in theme name, or a name registered earlier via Rayfield:AddTheme
-- (like "Neon Void" here), or a one-off table instead (see next button).
api:CreateDropdown({
    name     = "Theme",
    options  = { "Dark", "Blood Red", "Amethyst", "Rose", "Frost", "Cobalt", "Ember", "Gold", "Midnight", "Neon Void" },
    value    = "Midnight",
    callback = function(value) window:ChangeTheme(value) end,
})

-- A table passed straight to ChangeTheme is a one-off, unnamed theme: any key you don't set
-- falls back to the Dark theme's default. Use Rayfield:AddTheme instead when you want the
-- theme to have a name, be reusable, and appear in the built-in Settings tab's dropdown.
api:CreateButton({
    name     = "Apply One-off Theme Table",
    callback = function()
        window:ChangeTheme({
            AccentColor = Color3.fromRGB(80, 220, 140),
            WindowColor = Color3.fromRGB(15, 20, 18),
        })
    end,
})

-- window:ToggleWindowTransparency(bool) fades the whole window background. This is the
-- same function the built-in Settings tab's own transparency toggle calls internally.
api:CreateToggle({
    name     = "Window Transparency",
    callback = function(value) window:ToggleWindowTransparency(value) end,
})

api:CreateSection({ name = "Tags" })

-- window:CreateTag adds a small colored pill next to the window title.
-- Returns a Tag with :SetColor(color), :SetText(text), :SetIcon(icon), :Set({...}), :Remove().
local betaTag = window:CreateTag({ text = "BETA", color = Color3.fromRGB(255, 175, 15) })
api:CreateButton({ name = "Recolor Tag", callback = function() betaTag:SetColor(Color3.fromRGB(80, 200, 255)) end })
api:CreateButton({ name = "Remove Tag",  callback = function() betaTag:Remove() end })

api:CreateSection({ name = "Window state" })

-- window:Hide() collapses the window into the OpenButton pill; window:Show() restores it.
-- window:ToggleHide() flips between the two, and window:ToggleMinimise() only shrinks the topbar.
api:CreateButton({
    name     = "Hide Window (auto-reopens in 2s)",
    callback = function()
        window:Hide()
        task.delay(2, function() window:Show() end)
    end,
})
api:CreateButton({ name = "Toggle Minimise", callback = function() window:ToggleMinimise() end })

-- window:SetProfile(text) changes the small subtitle text under the sidebar avatar chip (UserInfo).
api:CreateButton({
    name     = "Set Profile Text",
    callback = function() window:SetProfile("Online — " .. os.date("%H:%M:%S")) end,
})

api:CreateSection({ name = "Flags" })

-- window:Get(flag) / window:Set(flag, value) read or write any flagged control from anywhere,
-- without keeping a reference to the control object. "LoadoutAimbot" is the flag set earlier
-- on the Layout tab's Aimbot toggle.
api:CreateButton({
    name     = "Read LoadoutAimbot Flag",
    callback = function()
        window:Notify({ title = "LoadoutAimbot = " .. tostring(window:Get("LoadoutAimbot")) })
    end,
})
api:CreateButton({
    name     = "Flip LoadoutAimbot Flag",
    callback = function() window:Set("LoadoutAimbot", not window:Get("LoadoutAimbot")) end,
})

api:CreateSection({ name = "Raw themed instances" })

-- window:Create(className, properties, themeProperties) makes an Instance that Rayfield tracks
-- (destroyed on Unload) and themes automatically. themeProperties maps a property name to a
-- theme key, so this bar recolors itself on every ChangeTheme call above.
local swatch = window:Create("Frame", {
    Size        = UDim2.fromOffset(0, 28),
    AutomaticSize = Enum.AutomaticSize.X,
    LayoutOrder = 9999,
    Parent      = api.tabPage,
}, {
    BackgroundColor3 = "AccentColor",
})
window:Create("UICorner", { CornerRadius = UDim.new(0, 6), Parent = swatch })

-- window:DestroySubtree(instance) removes an instance and everything under it, and forgets
-- it from the window's tracked instance/theme lists at the same time.
api:CreateButton({ name = "Destroy Swatch", callback = function() window:DestroySubtree(swatch) end })

api:CreateSection({ name = "Connections" })

-- window:Connect(signal, fn) wires a signal and remembers the connection so window:Unload()
-- cleans it up automatically later. window:Disconnect(connection) tears it down early.
local heartbeats = 0
local heartbeatStat = api:CreateStat({ name = "Heartbeats", value = 0 })
local heartbeatConnection = window:Connect(game:GetService("RunService").Heartbeat, function()
    heartbeats += 1
    if heartbeats % 30 == 0 then heartbeatStat:Set(heartbeats) end
end)
api:CreateButton({
    name     = "Disconnect Heartbeat Counter",
    callback = function() window:Disconnect(heartbeatConnection) end,
})

api:CreateSection({ name = "Custom translator" })

-- window:SetTranslator(fn) intercepts every locale lookup with your own (text, localeId) -> string
-- function, as an alternative to RegisterTranslations tables (e.g. for a live translation API).
api:CreateToggle({
    name     = "Prefix Labels via Translator",
    callback = function(value)
        window:SetTranslator(function(text, localeId)
            if value and localeId == "en" then return "» " .. text end
            return text
        end)
    end,
})

api:CreateSection({ name = "Teardown" })

-- window:Unload() disconnects every connection and destroys every instance the window ever
-- tracked via Create()/CreateTab()/etc. Irreversible — the entire UI is gone after this call.
api:CreateButton({ name = "Unload Window", callback = function() window:Unload() end })

-- window:Navigate("TabName" | tabObject) switches to that tab programmatically.
-- Accepts either the string name or the Tab object returned by CreateTab.
window:Navigate("Home")
