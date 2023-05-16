# Acceleration-TimePlot
# Using MATLAB to achieve a phenomenal acceleration time graph
# Three axis acceleration time graph
% Load data from Excel file
data = xlsread('abc.xlsx'); % replace with the name of your Excel file
% Assume the data is organized as follows: time, x1, y1, z1, x2, y2, z2, x3, y3, z3
time = data(:, 1);
x1 = data(:, 2);
y1 = data(:, 3);
z1 = data(:, 4);
x2 = data(:, 5);
y2 = data(:, 6);
z2 = data(:, 7);
x3 = data(:, 8);
y3 = data(:, 9);
z3 = data(:, 10);

% Plot acceleration-time graph for each sensor
figure;
subplot(3, 1, 1);
plot(time, x1, time, y1, time, z1);
title('Sensor 1 Acceleration');
legend('X', 'Y', 'Z');
xlabel('Time (s)');
ylabel('Acceleration (m/s^2)');
subplot(3, 1, 2);
plot(time, x2, time, y2, time, z2);
title('Sensor 2 Acceleration');
legend('X', 'Y', 'Z');
xlabel('Time (s)');
ylabel('Acceleration (m/s^2)');
subplot(3, 1, 3);
plot(time, x3, time, y3, time, z3);
title('Sensor 3 Acceleration');
legend('X', 'Y', 'Z');
xlabel('Time (s)');
ylabel('Acceleration (m/s^2)');
