#!/bin/bash

# Warp Theme Installer
# Author: vcalderon.dev
# Installs the "Trae AI Theme" into your Warp config directory

set -e

echo "📁 Creating ~/.warp/themes directory if it does not exist..."
mkdir -p "$HOME/.warp/themes"

echo "📄 Downloading trae-ai.yaml to ~/.warp/themes/"
curl -fsSL https://raw.githubusercontent.com/vcalderondev/trae-ai-warp-theme/main/trae-ai.yaml -o "$HOME/.warp/themes/trae-ai.yaml"

echo "✅ 'Trae AI Theme' installed at ~/.warp/themes/trae-ai.yaml"
echo "✨ Open Warp > Preferences > Appearance > Themes to activate it"