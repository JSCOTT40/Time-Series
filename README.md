# Time Series Generator and Filter Tool
Summary of Skills Learned Through PHYS 4060: Time series and Spectral Analysis, the code is being improved through a more interactive interface using pyQt5 however the overall mathematics and function of what is to be done remains the same. 

This Python script allows you to generate, visualize, and apply frequency-based filters to synthetic time series data. The tool is interactive, prompting the user for input parameters to define the characteristics of the time series, including frequencies, amplitudes, phases, and noise levels. Additionally, it provides options for filtering the time series using high-pass, low-pass, and band-pass filters.

## Features

Time Series Generation:
- Customize the number of sinusoidal components.
- Specify or randomize frequencies, amplitudes, and phases.
- Add white noise with configurable bounds.

Visualization:
- Plot the time series in the time domain.
- Compute and plot the Power Spectral Density (PSD) in the frequency domain.

Filtering Options:
- Apply high-pass, low-pass, and band-pass filters with user-defined cutoff frequencies.
- Visualize the effects of filters in both time and frequency domains.

### Dependencies

Ensure you have the following Python libraries installed:
- numpy
- matplotlib

You can install these libraries using pip:

```bash
pip install numpy matplotlib
```
#### Usage

Run the script in a Python environment. The script is interactive and will prompt you to provide inputs for generating the time series and applying filters.

**Example Workflow**:

- Generate a Time Series:
- Specify the number of sinusoidal components.
- Choose frequency, amplitude, and phase settings (random, set, or manual).
- Optionally, add white noise with specified bounds.
- Visualize the Time Series:
- View the time series in the time domain.
- Analyze the frequency domain using PSD plots.
- Apply Filters:
- Choose from high-pass, low-pass, or band-pass filters.
- Specify cutoff frequencies interactively.
- Compare the original and filtered series visually.

**Example Input and Output:**
```bash
How Many Sinusoids are in this Time Series? 5
What is the Starting Time? 0
What is the Final Time? 10
Do you want Random, Set or Manual frequency? Set
Do you want Random, Set or Manual Amplitude? Set
Do you want Random, Set or Manual Phase? Set
Do you want White Noise? Yes
Do you want Set or Manual White Noise? Set
```

**Generated plots**:

Time domain representation of the series.
Frequency domain representation (PSD).

**Filters:**

High-Pass Filter:
Removes frequencies below the specified cutoff.

Low-Pass Filter:
Removes frequencies above the specified cutoff.

Band-Pass Filter:
Retains frequencies within a specified range.

File Structure
The script contains the following key components:

**Functions**:
- floatcheck(S): Validates float inputs.
- intcheck(S): Validates integer inputs.
- Mean(S): Computes the mean of a series.
- autocov(Series, N, k): Computes autocovariance.
- PSD(S): Computes the Power Spectral Density (PSD).

**Interactive Inputs**:

Prompts the user to define time series parameters.
Filtering and Visualization:
High-pass, low-pass, and band-pass filter implementations.
Real-time plots for both time and frequency domains.

License

This project is open-source and available under the MIT License.

Contribution

Contributions are welcome! Feel free to fork the repository, submit issues, or create pull requests.
