#include <iostream>
#include <string>
using namespace std;

class SmartDevice {
private:
    int deviceId;
    string deviceType;
    string location;
    string status;
    string lastUpdated;

public:
    // Constructor
    SmartDevice(int id, string type, string loc, string stat, string time)
        : deviceId(id), deviceType(type), location(loc),
          status(stat), lastUpdated(time) {}

    // Switch device ON
    void switchOn(string time) {
        status = "ON";
        lastUpdated = time;
    }

    // Switch device OFF
    void switchOff(string time) {
        status = "OFF";
        lastUpdated = time;
    }

    // Change device status
    void changeStatus(string newStatus, string time) {
        status = newStatus;
        lastUpdated = time;
    }

    // Display device details
    void display() const {
        cout << "Device ID: " << deviceId << endl;
        cout << "Device Type: " << deviceType << endl;
        cout << "Location: " << location << endl;
        cout << "Status: " << status << endl;
        cout << "Last Updated: " << lastUpdated << endl;
        cout << "-----------------------------" << endl;
    }
};

int main() {

    // Create smart devices
    SmartDevice light(101, "Light", "Living Room", "OFF", "10:00 AM");
    SmartDevice thermostat(102, "Thermostat", "Bedroom", "ON", "10:05 AM");
    SmartDevice camera(103, "Camera", "Main Door", "ON", "10:10 AM");
    SmartDevice doorLock(104, "Door Lock", "Main Door", "LOCKED", "10:15 AM");

    // Perform operations
    light.switchOn("10:20 AM");
    thermostat.changeStatus("24 Degree C", "10:25 AM");
    camera.switchOff("10:30 AM");
    doorLock.changeStatus("UNLOCKED", "10:35 AM");

    // Display overall home dashboard
    cout << "========== SMART HOME DASHBOARD ==========" << endl;
    cout << endl;

    light.display();
    thermostat.display();
    camera.display();
    doorLock.display();

    return 0;
}
