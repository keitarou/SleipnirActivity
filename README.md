# SleipnirActivity

![Screenshot](./screenshot.png)

## Usage


    NSArray* activityItems = [NSArray arrayWithObjects:
                                [NSString stringWithFormat:@"Google"],
                                [NSURL URLWithString:@"http://google.com"],
                                nil
                              ];

    SleipnirActivity* sleipnirActivity             = [[SleipnirActivity alloc] init];

    UIActivityViewController *activityView = [[UIActivityViewController alloc]
                                               initWithActivityItems:activityItems
                                               applicationActivities:@[
                                                                       sleipnirActivity
                                                                       ]
                                              ];

    [self presentViewController:activityView animated:YES completion:^{

    }];

