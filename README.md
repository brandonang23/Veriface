# Veriface

Veriface is a proof-of-personhood face biometrics system I designed to prevent bots and automated abuse.

## Libraries Used

Veriface is built using **face-api.js**, a powerful library created by *justadudewhohacks* that runs on top of TensorFlow. This library utilizes a highly accurate machine learning model developed by Google.

It is designed to work in web browsers, though I'm not certain about its compatibility with Node.js or Express.js environments.

## How It Works

1. **Model Loading**: Veriface first loads the facial recognition model.
2. **Verification Process**: The system will prompt you to perform specific actions, such as turning your head or smiling.
3. **Face Descriptor Collection**: After successful verification, it collects a mathematical descriptor of your facial features.
4. **Profile Matching**: 
   - If you have an existing profile, Veriface compares your current face descriptor against the stored profile to verify your identity.
   - If you don't have a profile, the system automatically creates one using your facial data.
5. **Completion**: Once this process finishes, you're successfully verified.
