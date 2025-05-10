# CSE4310 Tracking Project

This project demonstrates object tracking and motion detection using video frames. It uses `skvideo` for video processing and PyQt6 (`pyside6`) for the GUI. The code tracks moving objects in parking lot videos and highlights them with bounding boxes.

## Requirements

### Python Environment

To run the project, you need to set up the required Python environment. This can be done by creating a Conda environment with the `environment.yml` file provided.

### Creating the Conda Environment

1. Clone or download the repository containing this README.

2. Navigate to the project folder in the terminal.

3. Create the Conda environment using the following command:

   ```bash
   conda env create -f environment.yml
   ```

4. Activate the environment:

   ```bash
   conda activate cse4310tracking
   ```

### Dependencies

* **PySide6**: For the GUI interface (based on Qt6).
* **NumPy**: For numerical operations.
* **scikit-video**: For video processing and object tracking.

If you have missing dependencies after the setup, you can install them manually:

```bash
conda install conda-forge::pyside6 numpy scikit-video
```

## Running the Script

### 1. Activate the Environment

If you haven't already activated the environment, do so by running:

```bash
conda activate cse4310tracking
```

### 2. Run the Object Tracking Script

Run the `ObjectTracking.py` script to process a video and track objects. The script will prompt you for the file path of the video.

Example:

```bash
python ObjectTracking.py
```

When prompted, enter the path to your video file:

```
/path/to/your/video.mp4
```

### 3. View the Results

The program will display the video with bounding boxes drawn around detected moving objects.

## Updating Environment

To ensure everything works seamlessly, here are some tips:

1. **Check FFmpeg Installation**:

   * Make sure `ffmpeg` is installed. If it's not, you can install it via Conda:

     ```bash
     conda install -c conda-forge ffmpeg
     ```

2. **Update NumPy**:

   * If you run into issues with deprecated features (e.g., `np.int`), ensure you're using the appropriate versions of NumPy or modify the code accordingly as described in the troubleshooting section.

3. **Script Modifications**:

   * If you encounter deprecated functions like `fromstring`, replace them with `np.frombuffer`.

## Demo Videos

You can view output here: [Google Drive Link](https://drive.google.com/file/d/1WyE7iOAEl_vCOsSoNojz0MKQ7bdH43Dm/view?usp=sharing)

## License

This project is licensed under the MIT License.
